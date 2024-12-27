<template>
  <div class="snowfall">
    <div
      v-for="flake in flakes"
      :key="flake.id"
      class="snowflake"
      :style="flake.style"
    ></div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const flakes = ref([]);

function createSnowflakes(count) {
  for (let i = 0; i < count; i++) {
    flakes.value.push({
      id: i,
      style: {
        left: `${Math.random() * 100}vw`,
        animationDelay: `${Math.random() * 5}s`,
        animationDuration: `${5 + Math.random() * 10}s`,
        transform: `scale(${0.5 + Math.random() * 0.2})`,
      },
    });
  }
}

onMounted(() => {
  createSnowflakes(50);
});
</script>

<style lang="less" scoped>
.snowfall {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  overflow: hidden;
  z-index: -99;
  
  & .snowflake {
    position: absolute;
    top: -5%;
    width: 5px;
    height: 5px;
    background-color: rgba(255, 255, 255, 0.288);
    border-radius: 50%;
    opacity: 0.8;
    animation-name: fall;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
}


@keyframes fall {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(100vh);
  }
}
</style>
