<template>
    <section class="p-about">
      <div class="l-container">
        <div class="p-about__title">about</div>
        <div class="p-about__intro">
          <h2 class="p-about__secHeading">php conference Kansai 2020</h2>
          <p class="p-about__read">
            集え、PHPer！！<br>
            PHPerのGWはこの日が本番<br>
            あのPHPの祭典がついに帰ってきた！<br><br>
            今回のテーマは「Share!!」<br><br>
            当日はPHPに関するトークセッションのほか、懇親会やその他イベントを実施予定<br>
            「PHPカンファレンス関西」で知識•技術•感動をみんなで分かち合おう！
          </p>
        </div>
        <div class="p-about__past">
          <h3 class="p-about__pastHeading">過去のイベントの様子はこちら</h3>
          <a class="p-about__pastList" href="https://2018.kphpug.jp/" target="_blank">2018</a>
          <a class="p-about__pastList" href="https://2017.kphpug.jp/" target="_blank">2017</a>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2016/" target="_blank">2016</a>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2015/" target="_blank">2015</a>
          <br>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2014/" target="_blank">2014</a>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2013/" target="_blank">2013</a>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2012/" target="_blank">2012</a>
          <a class="p-about__pastList" href="http://conference.kphpug.jp/2011/" target="_blank">2011</a>
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

.p-about {
  margin: 0 auto ;
  padding-bottom: 67px;
  position: relative;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;
  @include desktop {
    background-image:url("~assets/images/about/about_zou_left.png"),url("~assets/images/about/about_zou_right.png");
    background-position: bottom 20px left 6%,bottom 20px right 0px;
    background-repeat: no-repeat;
    padding-bottom: 100px;
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
    margin-bottom: 35px;
    @include desktop {
      text-align: center;
      padding: 50px 80px 90px 80px;
      font-size: 2.8rem;
      margin-bottom: 100px;
    }
  }

  &__secHeading {
    display: inline-block;
    text-align: center;
    letter-spacing: 1.12px;
    font-size: 1.6rem;
    margin-bottom: 20px;

    @include desktop {
    width: 434px;
    height: 39px;
    font-size: 2.8rem;
    margin-bottom: 45px;
    }


  }

  &__read {
    display: inline-block;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    font-size: 1.2rem;
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

  &__past {
    background-color: #FFFFFF;
    text-align: center;
    padding: 16px 0;
    border-radius: 50px;
    line-height: 1;
  }
  &__pastHeading {
    padding-bottom: 8px;
    font-size: 12px;
    @include desktop {
      font-size: 18px;
    }
  }
  &__pastList {
    margin-right: 20px;
    font-weight: bold;
    font-size: 12px;
    @include desktop {
      font-size: 18px;
    }
  }
  &__pastList:nth-child(5n) {
    margin-right: 0;
    @include desktop {
      margin-right: 20px;
    }
  }
  &__pastList:last-child {
    @include desktop {
      margin-right: 0;
    }
  }
  &__past br {
    @include desktop {
      display: none;
    }
  }
}

</style>
