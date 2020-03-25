<template>
    <section class="p-about">
      <div class="l-container">
        <div class="p-about__title">about</div>
        <div class="p-about__intro">
          <h2 class="p-about__secHeading">PHPカンファレンス関西2020とは</h2>
          <p class="p-about__read">
            PHPカンファレンス関西2020とは、PHPユーザ同士の交流によって、関西のPHPコミュニティを盛り上げることを目的とした、関西最大のPHPイベントです！！<br><br>
            普段PHPを使った開発をしている方はもちろん、PHPに興味がある人や、昔利用していた人、これから学ぼうとしている人から学生の方まで、PHPに関わるすべての人が対象です。<br><br>
            当日は一般公募された登壇者によるトークセッションや、懇親会をはじめとした、PHPに対する知識や理解を深め、参加者同士が交流できるような企画を開催します。
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
  padding-bottom: 40px;
  position: relative;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;
  @include desktop {
    background-image:url("~assets/images/about/about_zou_left.png"),url("~assets/images/about/about_zou_right.png");
    background-position: bottom 20px left 6%,bottom 20px right 0;
    background-repeat: no-repeat;
    padding-bottom: 100px;
  }

  &__title {
    @include c-section-title;
  }

  &__intro {
    background-color: #ffffff;
    border-radius: 10px;
    font-weight: bold;
    padding: 30px 20px 36px 20px;
    width: 100%;
    text-align: center;
    margin-bottom: 30px;
    @include desktop {
      border-radius: 0;
      padding: 50px 80px 90px 80px;
      font-size: 2.8rem;
      margin-bottom: 60px;
    }
  }

  &__secHeading {
    text-align: center;
    letter-spacing: 1.12px;
    font-size: 1.6rem;
    margin-bottom: 20px;
    @include desktop {
      height: 39px;
      font-size: 2.8rem;
      margin-bottom: 45px;
    }
  }

  &__read {
    font-weight: bold;
    text-align: center;
    font-size: 1.2rem;
    line-height: 2;
    @include desktop {
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
