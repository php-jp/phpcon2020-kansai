<template>
  <div class="c-hero">
    <div class="c-hero__wrapper l-container">
      <h2 class="c-hero__image">
        <img class="c-hero__logo" src="@/assets/images/hero/hero_logo.svg" alt="logo-img">
      </h2>
      <p class="c-hero__leadTxt">
        PHPカンファレンスが今年も開催！
      </p>
      <date class="c-hero__date">
        5/9
      </date>
      <p class="c-hero__location"><img src="@/assets/images/hero/place-24px.svg" class="c-hero__locationIcon" alt="location-pin" /> ブリーゼプラザ ホール&カンファレンス</p>
      <p class="c-hero__announce">スポンサー、登壇者募集開始！！</p>
      <div class="c-hero__buttons">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSfyrd-NmeeGTQke-2-KyBqXU2D10Hd7CcJheewBAd1Os6YIOA/viewform" class="c-hero__button" target="_blank" >スポンサー募集中</a>
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSc_4ulNeFqcBYOItbQR0EoCy0NR6EUYV_GhuttWhxLwgPuNWA/viewform" class="c-hero__button" target="_blank" >登壇者募集中</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {

};

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

$font-family:"M PLUS Rounded 1c";

  .c-hero {
    font-family: $font-family;
    color:$clr-accentcolor;
    width:100%;
    padding:66px 0 90px 0;
    position: relative;

    @include desktop {
      background-image: none;
      padding:66px 0 154px 0;
    }

    &::before {
      @include desktop {
        content: "";
        background-image: url('../../assets/images/hero/hero_zou_left.svg');
        background-size: 100%;
        background-repeat: no-repeat;
        width:40vw;
        min-width: 450px;
        height: 36vw;
        min-height: 380px;
        display: inline-block;
        position: absolute;
        top:39px;
        z-index: -100;
        left:39px;
      }
    }

    &::after {
      @include desktop {
        content:"";
        background-image:url('../../assets/images/hero/hero_zou_right.svg');
        background-size: 100%;
        background-repeat: no-repeat;
        width: 40vw;
        min-width: 450px;
        height: 36vw;
        min-height: 380px;
        display: inline-block;
        position: absolute;
        right:39px;
        bottom: 0;
        z-index: -100;
        
      }
    }

    &__wrapper {
      max-width: 610px;
      margin:0 auto;
      text-align: center;
      padding:0;
    }

    &__logo {
      width: 60%;
      height: 60%;
    }

    &__leadTxt  {
      @include desktop {
        font-size: 25px;
      }
      font-size: 15px;
      font-weight: bold;
      margin-top:32px;
    }

    &__date {
      font-size: 43px;
      line-height: 1;
      letter-spacing: 2.5px;
      font-weight: bold;
      position: relative;
      margin:30px 0 16px 0;
      display: inline-block;

      &::after {
        @include desktop {
          width:40px;
          height:38px;
          font-size: 20px;
          font-weight: bold;
          padding-right: 1px;
        }
        content:"土";
        letter-spacing: 0px;
        width:36px;
        height:36px;
        font-size: 1.7rem;
        font-weight: bold;
        line-height: 2;
        border-radius: 50%;
        position: absolute;
        top:5px;
        margin-left:20px;
        color:#fff;
        background-color:$clr-accentcolor;

      }
    }


    &__location {
      font-size: 15px;
      font-weight: bold;
      line-height: 1.2;
      text-align: center;
      @include desktop {
        font-size: 24px;
        line-height: 1.3;
      }

    }

    &__locationIcon {
      text-align: center;
      width: 17px;
      height: 17px;
      @include desktop {
        line-height: 2;
        width: 30px;
        height: 30px;
      }
    }

    &__announce {
      font-size: 15px;
      font-weight: bold;
      background-color: #FAEFEC;
      min-width:280px;
      display: inline-block;
      margin: 0 auto;
      margin-top:30px;
      padding: 5px 0px 5px 0px;
      @include desktop {
        width:460px;
        font-size: 23px;
        margin-top:46px;
      }
    }

    &__buttons {
      display: flex;
      margin: 0 auto;
      margin-top: 20px;
      width: 280px;
      @include desktop {
        width: 100%;
      }
    }

    &__button {
      width: 140px;
      box-sizing: border-box;
      text-decoration: none;
      font-size: 1.3rem;
      color:#fff;
      font-weight: bold;
      line-height: 1.4;
      height: 40px;
      padding: 10px 9px 9px 10px;
      background-color: $clr-accentcolor;
      border-radius: 10px 9px 9px 10px;
      display: inline-block;
      &:nth-child(1) {
        margin-right: 20px;
        @include desktop {
          margin-right: 40px;
        }
      }
      @include desktop {
        width:280px;
        font-size: 20px;
        padding:17px 0;
        height: 60px;
      }
    }


  }
</style>


