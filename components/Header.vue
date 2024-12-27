<template>
  <header class="header farro-light">
		<div class="logo">
			<NuxtLink to="/"><img src="../assets/images/ООН logo1.png" alt=""/></NuxtLink>
		</div>
    
    <nav class="nav">
      <ul>
        <li><NuxtLink to="/">Главная</NuxtLink></li>
        <li><NuxtLink to="/invite">Как вступить?</NuxtLink></li>
        <li><NuxtLink to="/about">О нас</NuxtLink></li>
        <li><NuxtLink to="/rules">Правила</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="less" scoped>
  .header {
    padding: 20px 80px;
    display:flex;
    align-items: center;
    justify-content: center;
    & .logo {
      margin-right: auto;  
    }
    
    & .nav {
      
      & > ul {
        display: flex;
        gap: 40px;
        
        & > li {
          
          & > a {
            color: #fff;
            font-size: 18px;
          }
        }
      }
    }
    @media (max-width: 600px) {
      padding: 20px 20px;
      
      & .logo {
        margin-right: auto;  
        
        & > a {
          
          & > img {
            width: 70px;
          }
        }
      }
  
      & .nav {
        margin-left: 50px;
        & > ul {
          display: flex;
          gap: 10px;
          flex-wrap: wrap;
  
          & > li {
  
            & > a {
              color: #fff;
              font-size: 15px;
            }
          }
        }
      }
    }
  }
</style>