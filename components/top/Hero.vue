<template>
  <div class="c-hero">
    <div class="c-hero__wrapper c-container">
      <h2>
      <img src="@/assets/images/hero/hero_logo.svg" alt="logo-img">
      </h2>
      <p class="c-hero__leadTxt">
        PHPカンファレンスが今年も開催！
      </p>
      <date class="c-hero__date">
        5/9
      </date>
      <p class="c-hero__location"><img src="@/assets/images/hero/place-24px.svg" class="c-hero__locationIcon" alt="location-pin" /> ブリーゼプラザ ホール&カンファレンス</p>
      <p class="c-hero__announce">スポンサー、登壇者募集開始</p>
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

    &::before {
      content:"";
      background-image:url('../../assets/images/hero/hero_zou_left.svg');
      width:792px;
      height: 635px;
      display: inline-block;
      position: absolute;
      top:0;
      z-index: -100;
    }

    &::after {
       content:"";
      background-image:url('../../assets/images/hero/hero_zou_right.svg');
      width:792px;
      height: 635px;
      display: inline-block;
      position: absolute;
      right:0;
      bottom:0;
      z-index: -100;
    }


    

    &__wrapper {
      max-width: 610px;
      margin:0 auto;
      text-align: center;
      padding:0;
    }

    &__leadTxt  {
      font-size: 25px;
      font-weight: bold;
      margin-top:32px;

    }
    &__date {
      font-size: 66px;
      line-height: 1;
      font-weight: bold;
      position: relative;
      margin:30px 0 16px 0;
      display: inline-block;

      &::after {
        content:"土";
        width:55px;
        height:55px;
        font-size: 28px;
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
      font-size: 24px;
      font-weight: bold;
      line-height: 1.3;
    }

    &__locationIcon {
      line-height: 2;
    }

    &__announce {
      font-size: 23px;
      font-weight: bold;
      background-color: #FAEFEC;
      width:460px;
      display: inline-block;
      margin: 0 auto;
      margin-top:46px;
    }

    &__buttons {
      margin-top:30px;
    }

    &__button {
      text-decoration: none;
      font-size: 20px;
      color:#fff;
      width:280px;
      font-weight: bold;
      line-height: 1.4;
      height: 60px;;
      background-color: $clr-accentcolor;
      padding:17px 0;
      border-radius: 10px;
      display: inline-block;
      &:nth-child(1) {
        margin-right: 40px;
      }
    }
    
    
  }
</style>


