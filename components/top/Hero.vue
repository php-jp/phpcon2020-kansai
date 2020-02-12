<template>
  <div class="c-hero">
    <div class="c-hero__wrapper c-container">
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
        <a href="" class="c-hero__button">スポンサー募集中</a>
        <a href="" class="c-hero__button">登壇者募集中</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

$font-family:"M PLUS Rounded 1c";


  .c-hero {
    font-family: $font-family;
    color:$clr-accentcolor;
    width:100%;
    position:relative;
    background-image: url('~assets/images/hero/hero_sp_zou.png');
    background-repeat: no-repeat;
    background-size: cover;

    @include desktop {
      background-image: none;
    }

    &::before {
      @include desktop {
        content: "";
        background-image: url('../../assets/images/hero/hero_zou_left.svg');
        background-attachment: fixed;
        background-repeat: no-repeat;
        width:792px;
        height: 635px;
        display: inline-block;
        position: absolute;
        top:0;
        z-index: -100;
      }
    }

    &::after {
      @include desktop {
        content:"";
        background-image:url('../../assets/images/hero/hero_zou_right.svg');
        background-attachment: fixed;
        background-repeat: no-repeat;
        width:792px;
        height: 635px;
        display: inline-block;
        position: absolute;
        right:0;
        bottom:0;
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
        width:36px;
        height:36px;
        font-size: 17px;
        font-weight: bold;
        line-height: 1.8;
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
      @include desktop {
        width:460px;
        font-size: 23px;
        margin-top:46px;
      }
    }

    &__buttons {
      margin: 0 auto;
      margin-top: 30px;
      width: 280px;
      @include desktop {
        width: 100%;
      }
    }

    &__button {
      box-sizing: border-box;
      text-decoration: none;
      font-size: 15px;
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


