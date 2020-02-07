<template>
  <section>
    <div class="p-about">
      <div class="c-container">
        <div class="p-about_title">About</div>
        <div class="p-about_intro">
          <h1 class="p-about_secHeading">php conference Kansai 2020</h1>
          <p class="p-about_read">
            関西PHPerの夏はこれがなくちゃ始まらない！
            今年で８回目となる関西最大級のPHPイベント、今年も開催です。<br>
            全国PHPerが大阪に集結「PHPカンファレンス関西」で心に残る夏の思い出を！
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
  margin: 50px auto 0;
  position: relative;
  // background-image:
  //         url("~assets/img/about_frame01.png"),
  //         url("~assets/img/about_frame02.png");
  background-color: $clr_basecolor;
  background-size: 15%, 15%, 30%, 30%;
  background-position: left top, right bottom, 45% 0%, 50% 100%;
  background-repeat: no-repeat;
  color: $clr_accentcolor;

  @include desktop {
    margin-top: 100px;
    background-size: 15%, 15%, 15%, 18%;
  }

  &_title {
    @include c-section-title;
  }

  &_intro {
    background-color: #ffffff;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    display: inline-block;
    padding: 50px 80px 90px 80px;
    width: 100%;
    text-align: left;
    font-size: 2.8rem;
    margin-bottom: 100px;
    @include desktop {
      text-align: center;
      font-size: 2.8rem;
    }
  }

  &_secHeading {
    font-size: 2.8rem;
    margin-bottom: 45px;

  }

  &_read {
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    font-size: 1.8rem;
    line-height: 2;
  }
}

</style>
