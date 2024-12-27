<template>
  <footer class="footer farro-light">
    <div class="logo">
      <img src="../assets/images/ООН logo1.png" alt="">
    </div>

    <div class="links">

      <nav class="nav-pages">
        <ul>
          <li><NuxtLink to="/">Главная</NuxtLink></li>
          <li><NuxtLink to="/invite">Как вступить?</NuxtLink></li>
          <li><NuxtLink to="/about">О нас</NuxtLink></li>
          <li><NuxtLink to="/rules">Правила</NuxtLink></li>
        </ul>
      </nav>

      <nav class="nav-contacts">
        <a href="https://t.me/hvnttr">Тг создателя ООН</a>
        <p>ceoofunitednations@gmail.com</p>
      </nav>
    </div>
  </footer>
</template>

<style lang="less" scoped>
  a {
    text-decoration: underline;
  }
  .footer {
    margin-top: 50px;
    padding: 50px 50px;
    background: #000;
    height: 20vh;
    display: flex;
    position: relative;
    & .logo {
      position: absolute;
      right: 30px;
      top: 20px;
    }

    & .links {
      display: flex;
      justify-content: space-between;

      & .nav-pages {
        margin-right: 500px;
        & > li {
          margin-bottom: 10px;
        }
      }
    }
    
    @media (max-width: 600px) {
      margin-top: 20px;
      padding: 20px 20px;
      background: #000;
      display: flex;
      position: relative;

      & .logo {
        position: absolute;
        right: 1%;
        top: 70%;
        & > img {
          width: 50px;
        }
      }
  
      & .links {
        display: flex;
        justify-content: space-between;
        
        & .nav-pages {
          margin-right: 25px;
          & > ul {
            & > li {
              & > a {
                font-size: 15px;
              }
              margin-bottom: 0px;
            }
          }
        }

        & .nav-contacts {
          & > a {
            font-size: 15px;
          }
          & > p {
            font-size: 15px;
          }
        }
      }
      
    }
  }
</style>