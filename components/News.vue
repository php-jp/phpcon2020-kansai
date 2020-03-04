<template>
    <section class="p-news">
      <div class="l-container">
        <div class="p-news__title">news</div>
        <div class="p-news__intro">
          <h2 class="p-news__secHeading">新型コロナウィルス感染症に関する対応方針について</h2>
          <p class="p-news__read">
            PHPカンファレンス関西は予定通り5月9日（土）に開催することを目指して準備を進めています。<br>
            ただし、今後の状況により、イベントの自粛などが必要と判断した場合には、不本意ながらイベント自体の延期、または中止を判断する可能性もありますので、予めご了承ください。<br>
            しかしながら、現時点で5月の開催是非を決定できるための十分な情報がなく、また時間の猶予もあることから、現在は予定通り開催に向けて準備を進めております。<br>
            運営委員会としては、引き続き状況を注視しつつ、全関係者にとって最善の選択ができるよう、検討と判断をしていきます。
          </p>
        </div>
      </div>
    </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-news {
  margin: 0 auto ;
  position: relative;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;
  @include desktop {
    background-image:url("~assets/images/about/about_zou_left.png"),url("~assets/images/about/about_zou_right.png");
    background-position: bottom 20px left 6%,bottom 20px right 0px;
    background-repeat: no-repeat;
  }

  &__title {
    @include c-section-title;

  }

  &__intro {
    background-color: #ffffff;
    border-radius: 10px;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    @include desktop {
      border-radius: 0px;
    }
    display: inline-block;
    padding: 30px 20px 36px 20px;
    width: 100%;
    text-align: center;
    margin-bottom: 100px;
    @include desktop {
      text-align: center;
      padding: 50px 80px 90px 80px;
      font-size: 2.8rem;
      margin-bottom: 200px;
    }
  }

  &__secHeading {
    display: inline-block;
    text-align: center;
    letter-spacing: 1.12px;
    font-size: 1.6rem;
    margin-bottom: 20px;

    @include desktop {
    height: 39px;
    font-size: 2.8rem;
    margin-bottom: 45px;
    margin-top: 25px;
    }


  }

  &__read {
    display: inline-block;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    font-size: 1.3rem;
    line-height: 2;
    @include desktop {
    display: inline-block;
    width: 683px;
    height: 115px;
    text-align: center;
    font-size: 1.8rem;
    line-height: 2;
    }
  }
}

</style>
