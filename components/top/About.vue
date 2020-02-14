<template>
  <section>
    <div class="p-about">
      <div class="l-container">
        <div class="p-about_title">about</div>
        <div class="p-about_intro">
          <h1 class="p-about_secHeading">php conference Kansai 2020</h1>
          <p class="p-about_read">
            関西PHPerの夏はこれがなくちゃ始まらない！<br>
            今年で８回目となる関西最大級のPHPイベント、今年も開催です。<br>
            <br>全国PHPerが大阪に集結「PHPカンファレンス関西」で心に残る夏の思い出を！
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-about {
  margin: 0 auto ;
  position: relative;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;
  @include desktop {
    background-image:url("~assets/images/about/about_zou_left.png"),url("~assets/images/about/about_zou_right.png");
    background-position: bottom 20px left 0px,bottom 20px right 0px;
    background-repeat: no-repeat;
  }

  &_title {
    @include c-section-title;

  }

  &_intro {
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

  &_secHeading {
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

  &_read {
    display: inline-block;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    // width: 240px;
    //height: 162px;
    text-align: center;
    font-size: 1.2rem;
    line-height: 2;
    @include desktop {
    display: inline-block;
    color: $clr_accentcolor;
    width: 683px;
    height: 115px;
    text-align: center;
    font-size: 1.8rem;
    line-height: 2;
    }
  }
}

</style>
