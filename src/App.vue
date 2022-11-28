<template>
  <div class="main">
    <div class="main__wrapper">
      <div class="main__header">
        <div class="main__header__container">
          <div class="main__header__column">
            <h1 class="">Привет, друг!</h1>
            <div class="main__header__column__check">
              <p>У тебя все получится!</p>
            </div>
            <p>Никогда не сдавайся!</p>
            <p>Сегодня ты уже знаешь больше чем вчера!</p>
            <p>Спасибо тебе за поддержку!</p>
          </div>
          <div class="main__header__column">
            <div class="main__header__img">
              <img src="./assets/1.png" />
            </div>
          </div>
        </div>
      </div>
      <div class="main__body">
        <div class="main__body__what">
          <div class="main__body__what__container">
            <div class="main__body__what__wrapp">
              <div class="main__body__what__column">
                <img src="./assets/what.png"/>
              </div>
              <div class="main__body__what__column">
                <h2 class="title">Что такое FlexBox?</h2>
                <p>Flexbox - это целый модуль, содержащий в себе набор свойств и их значений как для родителя flex-контейнера так и для его дочерних элементов flex-элементов. </p>
                <p>Основным преимуществом гибкой FLEX разметки является возможность изменять ширину/высоту пространство вокруг и порядок flex-элементов, для того чтобы наилучшим образом заполнить доступное пространство flex-контейнера</p>
              </div>
            </div>
          </div>
        </div>
        <div class="main__body__vertical-align">
          <div class="main__body__vertical-align__container">
            <h2 class="title">Вертикальное выравнивание</h2>
            <div class="main__body__vertical-align__row">
              <div class="main__body__vertical-align__row__wrapp">
                <div class="main__body__vertical-align__row__item">
                  <h3 class="main__body__vertical-align__row__item-title">буду рад</h3>
                  <p class="main__body__vertical-align__row__item-subtitle">подписке</p>
                  <p class="main__body__vertical-align__row__item-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint tenetur fugit vel, eligendi illum, placeat quo vero reiciendis consectetur.</p>
                  <button type="button" class="main__body__vertical-align__row__item-button">подписаться</button>
                </div>
                <div class="main__body__vertical-align__row__item">
                  <h3 class="main__body__vertical-align__row__item-title">буду рад</h3>
                  <p class="main__body__vertical-align__row__item-subtitle">лайку</p>
                  <p class="main__body__vertical-align__row__item-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint tenetur fugit vel, eligendi illum, placeat quo vero reiciendis consectetur voluptatibus atque et itaque, hic, deleniti. Sunt commodi tempora voluptatum dolorum.</p>
                  <p class="main__body__vertical-align__row__item-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint tenetur fugit vel, eligendi illum, placeat quo vero reiciendis consectetur tempora voluptatum dolorum.</p>
                  <button type="button" class="main__body__vertical-align__row__item-button">лайк</button>
                </div>
                <div class="main__body__vertical-align__row__item">
                  <h3 class="main__body__vertical-align__row__item-title">буду рад</h3>
                  <p class="main__body__vertical-align__row__item-subtitle">подписке</p>
                  <p class="main__body__vertical-align__row__item-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint tenetur fugit vel, eligendi illum, placeat quo vero reiciendis consectetur.</p>
                  <button type="button" class="main__body__vertical-align__row__item-button">комментировать</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="main__footer">
        <p>Фрилансер по жизни 2019</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    mounted() {
      console.log(window.flex)
    }
  }
</script>

<style lang="scss">
  .main {
    font-family: Arial, Helvetica, sans-serif;
    &__wrapper {
      // background-color: aquamarine;
      // padding: 20px;
      min-height: 100vh;
      overflow: hidden;
      display: flex;
      flex-direction: column;
    }
    &__header {
      color: #fff;
      // background-color: rgb(206, 113, 214);
      background-color: rgb(68, 81, 98);
      &__container {
        max-width: 1180px;
        margin: 0 auto;
        background-color: rgb(68, 81, 98);
        display: flex;
      }
      &__column {
        flex: 1 1 50%;
        margin: 50px;
      }
      h1 {
        margin: 0 0 30px 0;
        font-size: 40px;
        font-weight: 100;
      }
      &__img {
        width: 40%;
        img {
          max-width: 470px;
          max-height: 210px;
        }
      }
    }
    &__body {
      // background-color: rgb(143, 170, 23);
      flex: 1 0 auto;
      padding-bottom: 50px;
      &__what {
        &__container {
          max-width: 1180px;
          background-color: #fff;
          margin: 0 auto;
          // display: flex;
          padding: 50px;
          box-sizing: border-box;
        }
        &__wrapp {
          display: flex;
          overflow: hidden;
          align-items: center;
        }
        &__column {
          // background-color: aqua;
          flex: 1 1 auto;
          &:first-child {
            margin-right: 20px;
            flex: 0 0 430px;
          }
          h2 {
            color: rgb(68, 81, 98);
            font-weight: 200;
            margin: 0 0 30px 0;
          }
          p {
            color: #333333;
          }
        }
      }
      &__vertical-align {
        &__container {
          background-color: #fff;
          max-width: 1000px;
          margin: 0 auto;
          .title {
            color: rgb(68, 81, 98);
            font-weight: 200;
            margin: 0 0 30px 0;
            text-align: center;
          }
        }
        &__row {
          display: flex;
          justify-content: center;
          // background-color: red;
          // flex-wrap: wrap;
          &__wrapp {
            margin: 0 auto;
            display: flex;
            flex-wrap: wrap;
            // background-color: blue;
            justify-content: space-around;
            // width: max-content;
          }
          &__item {
            background-color: rgb(68, 81, 98);
            max-width: 300px;
            border-radius: 5px;
            color: #fff;
            border: 1px solid rgb(68, 81, 98);
            display: flex;
            flex-direction: column;
            margin: 15px;
            min-width: 100px;
            &-title {
              text-transform: uppercase;
              font-size: 20px;
              text-align: center;
              font-weight: normal;
            }
            &-subtitle {
              background-color: #fff;
              color: #333333;
              text-transform: uppercase;
              font-size: 26px;
              line-height: 50px;
              text-align: center;
            }
            &-text {
              margin: 10px;
              flex: 1 1 auto;
            }
            &-button {
              margin: 10px;
              border-radius: 5px;
              line-height: 36px;
              border: none;
              font-size: 20px;
              color: #333333;
            }
          }
        }
      }
    }
    &__footer {
      background-color: rgb(197, 197, 197);
      text-align: center;
      color: #333333;
    }
  }
  @media (max-width: 800px) {
    .main__header__container {
      flex-direction: column;
      padding: 20px;
      text-align: center;
    }
    .main__header__column {
      margin: 0 auto;
    }
    .main__body__what__wrapp {
      flex-direction: column;
    }
    .main__body__what__column:first-child {
      flex: 0 1 auto;
      margin-bottom: 50px;
      img {
        width: 100%;
      }
    }
  }
</style>