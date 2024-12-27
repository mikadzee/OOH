<template>
  <section class="main farro-light">
    <div class="main-container">
      <div class="general">
        <p>Добро пожаловать в Организацию Объединенных Наций (ООН) на сервере BixLand! Мы — международная организация, объединяющая города и нации для сотрудничества, мира и развития. Здесь вы найдете информацию о нашей деятельности, правилах и возможностях вступления.
        <br>
        Наша цель — создать процветающее и мирное сообщество на сервере, где каждый город может развиваться без конфликтов и с поддержкой других членов ООН. Мы стремимся к сотрудничеству в сфере экономики, культуры и безопасности.</p>

        <img src="../assets/images/image 1.png" alt="">
      </div>

      <div class="about-minimal">
        <h2>Введение</h2>

        <p>На сервере BixLand царила разрозненность. Города жили по своим законам, поселения старались выжить самостоятельно, а независимые игроки избегали крупных сообществ. Каждый занимался своим делом: кто-то строил огромные базы, кто-то прокладывал торговые маршруты, а кто-то жил в тени, исследуя неизведанные уголки мира.<br>Однако этот хаотичный порядок скрывал серьёзные проблемы. Отсутствие координации между игроками приводило к тому, что ресурсы распределялись несправедливо, а мелкие сообщества часто оставались <span>беззащитными</span>. Новички, едва начав своё путешествие, <span>быстро покидали сервер, не выдерживая давления.</span><br>Мир нуждался в изменениях, но никто не знал, с чего начать. Именно в этот переломный момент три лидера — странник, дипломат и стратег, обладавший огромным влиянием на развитие сервера — стали теми, кто изменил ход истории. Их действия положили начало созданию структуры, которая объединила всех и сделала BixLand местом, где каждый мог найти своё место.</p>
      </div>

      <div class="mains-peoples">
        <h2>Главные органы ООН:</h2>

        <div class="peoples">
          <div class="people">
            <a href="https://t.me/+S84BPVoW6mozNzYy" target="_blank">
              <img src="../assets/images/image 2.png" alt="">
              <p>Baha_ZXC</p>
            </a>
          </div>
          <div class="people">
            <a href="https://t.me/+S84BPVoW6mozNzYy">
              <img src="../assets/images/image 3.png" alt="">
              <p>26052003lll</p>
            </a>
          </div>
          <div class="people">
            <a href="https://t.me/+S84BPVoW6mozNzYy">
              <img src="../assets/images/zombiemask-1200x1200 1.png" alt="">
              <p>DetGeto</p>
            </a>
          </div>
        </div>
      </div>

      <div class="what-join">
        <h2>Как попасть в ООН?</h2>

        <p>Мы приглашаем города, которые разделяют наши ценности и готовы к сотрудничеству, присоединиться к нам. Чтобы узнать, как подать заявку на вступление, посетите страницу <NuxtLink to="/invite">"Вступление"</NuxtLink>.</p>
      </div>
    </div>
  </section>
</template>

<style lang="less" scoped>
  .main {
    
    & .main-container {
      margin: 0px 100px;

      @media (max-width: 600px) {
        margin: 0px 10px;

        & .general {
          display: flex;
          justify-content: space-between;
          align-items: center;
          
          & > p {
            width: 700px;
            font-size: 18px;
            line-height: 35px;
          }
  
          & > img {
            width: 35%;
            display: none;
          }
        }
  
        & .about-minimal {
          margin-top: 130px;
  
          & > h2 {
            margin-bottom: 25px;
            font-size: 20px;
          }
          
          & > p {
            font-size: 18px;
            line-height: 30px;
            & > span {
              color: red;
            }
          }
        }
  
        & .mains-peoples {
          margin-top: 130px;
          
          & > h2 {
            margin-bottom: 25px;
            font-size: 20px;
          }
  
          & .peoples {
            display: flex;
            justify-content: center;
            gap: 20px;
            align-items: center;
            flex-wrap: wrap;
            
            & .people {
              cursor: pointer;
  
              & > a {
                color: #fff;
                & > img {
                  width: 120px;
                }
                
                & > p {
                  margin-top: 10px;
                  text-align: center;
                }
              }
  
            }
          }
        }
  
        & .what-join {
          margin-top: 130px;
  
          & > h2 {
            margin-bottom: 25px;
            font-size: 20px;
          }
  
          & > p {
            margin-top: 10px;
            margin-left: 10px;
            font-size: 18px;
          }
        }
      }
      }
      
      & .general {
        display: flex;
        justify-content: space-between;
        align-items: center;
        
        & > p {
          width: 700px;
          font-size: 20px;
        }

        & > img {
          width: 35%;
          @media (max-width: 600px) {
            display: none;
          }
        }
      }

      & .about-minimal {
        margin-top: 130px;

        & > h2 {
          margin-bottom: 25px;
        }
        
        & > p {
          font-size: 20px;
          line-height: 30px;
          & > span {
            color: red;
          }
        }
      }

      & .mains-peoples {
        margin-top: 130px;
        
        & > h2 {
          margin-bottom: 25px;
        }

        & .peoples {
          display: flex;
          justify-content: center;
          gap: 150px;
          align-items: center;

          & .people {
            cursor: pointer;

            & > a {
              color: #fff;
              
              & > p {
                margin-top: 10px;
                text-align: center;
              }
            }

          }
        }
      }

      & .what-join {
        margin-top: 130px;

        & > h2 {
          margin-bottom: 25px;
        }

        & > p {
          margin-top: 10px;
          margin-left: 10px;
          font-size: 20px;

          & > a {
            color: aqua;
            text-decoration: underline;
          }
        }
      }
    }  
</style>