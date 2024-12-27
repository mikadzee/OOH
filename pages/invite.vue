<template>
  <section class="main farro-light">
    <div class="main-container">
      <h2>Как вступить?</h2>

      <div class="answer">
        <p>Чтобы стать членом Организации Объединенных Наций, ваш город должен соответствовать следующим критериям:</p>

        <ol>
          <li>* [Критерий 1]</li>
          <li>* [Критерий 2]</li>
          <li>* [Критерий 3]</li>
        </ol>
      </div>

      <div class="procedure">
        <h2>Процедура вступления:</h2>

        <ol>
          <li>Подача заявки: Мэр города подает заявку на вступление в ООН через <a href="https://t.me/hvnttr">Telegram</a>.</li>
          <li>Рассмотрение заявки: Заявка рассматривается Советом Безопасности ООН.</li>
          <li>Голосование: После рассмотрения заявки, Генеральная Ассамблея проводит голосование.</li>
          <li>Принятие в ООН: После одобрения заявки, город официально становится членом ООН.</li>
        </ol>
      </div>

      <div class="contacts">
        <h2>Свяжитесь с нами:</h2>

        <ol>
          <li><a href="https://t.me/hvnttr">Telegram</a></li>
          <li>Gmail ceoofunitednations@gmail.com</li>
        </ol>
        <p>Для получения дополнительной информации или подачи заявки.</p>
      </div>
    </div>
  </section>
</template>

<style lang="less" scoped>
  .main {

    & .main-container {
      margin: 0 100px;

      & > h2 {
        font-weight: 700;
        font-size: 40px;
        color: #7F7F7F;
      }

      & .answer {
        margin-top: 10px;
        font-size: 18px;
        & > h2 {
          font-size: 20px;
        }

        & > ol {

          & > li {
            
          }
        }
      }
      
      & .procedure {
        margin: 50px 0px;
      }

      @media (max-width: 600px) {
        margin: 0 10px;
        font-size: 18px;

        
      }
    }
  }
  a {
    color: aqua;
    text-decoration: underline;
  }
</style>