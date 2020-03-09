
<template>
  <section>
    <div class="p-session">
      <div class="l-container" >
        <div class="p-session_title">session</div>
          <p class="p-session_read">
            FRONTEND CONFERENCE 2019 セッション一覧公開中！<br>
            昨年同様、幅広いテーマの登壇内容を集めた珠玉のセッション構成で、 デザイナもエンジニアも、職種問わずWebに携わるすべての人が楽しめる内容となっています。<br>
          </p>
          <div class="p-session__button">
          <a href="" target ="_blank" >session一覧</a>
          </div>
        </div>
      </div>
    
  </section>
</template>


<style lang="scss" scoped>
@import "~/assets/scss/common.scss";
 $font-family:"M PLUS Rounded 1c";


    .p-session {
    position: relative;
    color: $clr_accentcolor;
    background-color: #FFFAF8;
    text-align: center;
    display: inline-block;

    &_title {
    @include c-section-title;
    }
    &_read {
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    font-size: 1.8rem;
    line-height: 3;
    @include desktop {
    display: inline-block;
    color: #F29B85;
    text-align: center;
    font-size: 1.8rem;
    line-height: 2;
    }
    }


    &__button {
    box-sizing: border-box;
    text-decoration: none;
    font-size: 1.8rem;
    color:#fff;
    font-weight: bold;
    line-height: 1.4;
    padding: 10px 0px 10px 10px;
    background-color: $clr-accentcolor;
    border-radius: 10px 9px 9px 10px;
    margin: 0 auto;
    margin-bottom: 100px;
    &:nth-child(1) {
    margin-right: 20px;
    @include desktop {
      margin-right: 40px;
    }
    }
    @include desktop {
    text-align: center;
    margin-top: 55px;

    width:260px;
    font-size: 20px;
    height: 55px;
    }
    }

   
}
</style>


</style>
