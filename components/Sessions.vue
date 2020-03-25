<template>
  <section class="p-sessions">
    <div class="l-container">
      <div class="p-sessions__title">sessions</div>
      <p class="p-sessions__sentence">
        フロントエンドのエンジニアリングや、マークアップ、デザインなど、<br>
        Webに関わる全ての人に是非届けたい珠玉のセッション構成でお送りしております。
      </p>
      <div class="p-sessions__card">
        <div class="p-sessions__details">
          <div class="p-sessions__location">
            <span class="p-sessions__roomNumber">A-1</span>
            <span class="p-sessions__time">11:00~</span>
          </div>
          <div class="p-sessions__sessionTitle">タイトルが入ります。25文字以内でお願いします。</div>
          <div class="p-sessions__sessionSubTitle">- サブタイトルがある場合はこのエリアに入ります。</div>
          <p class="p-sessions__description">
            (200文字程度)セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。セッションの概要が入ります。
          </p>
        </div>
        <hr class="p-sessions__hr">
        <div class="p-sessions__speaker">
          <div class="p-sessions__speakerSns">
            <img
              class="p-sessions__speakerImg"
              src="~assets/images/speaker/profileImg@2x.png"
              alt="speaker"
            >
            <div class="p-sessions__follow">
              <a
                class="p-sessions__link"
                href="https://www.facebook.com/pcon.kansai/"
                target="branck"
              >
                <img
                  class="p-sessions__followIcon"
                  src="~assets/images/footer/footer_icon_facebook.svg"
                  alt="facebook"
                />
              </a>
              <a
                class="p-sessions__link"
                href="https://twitter.com/phpcon_kansai"
                target="branck"
              >
                <img
                  class="p-sessions__followIcon"
                  src="~assets/images/footer/footer_icon_twitte.svg"
                  alt="twitter"
                />
              </a>
            </div>
          </div>
          <div class="p-sessions__speakerDescription">
            <div class="p-sessions__speakerName">山田太郎</div>
            <div class="p-sessions__speakerCompany">株式会社chatbox</div>
            <p class="p-sessions__description">
              (150文字以内)登壇者紹介文が入ります。登壇者紹介文が入ります。登壇者紹介文が入ります。登壇者紹介文が入ります。登壇者紹介文が入ります。登壇者紹介文が入ります。登壇者紹介文が入ります。
            </p>
          </div>
        </div>
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

.p-sessions {
  margin: 0 auto;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;

  &__title {
    @include c-section-title;
  }

  &__sentence {
    font-size: 12px;
    font-weight: bold;
    margin-bottom: 25px;
    @include desktop() {
      text-align: center;
      font-size: 23px;
      margin-bottom: 80px;
    }
  }

  &__card {
    width: 100%;
    padding: 47px 20px 86px;
    background-color: #FFFFFF;
  }

  &__details {
    margin-bottom: 52.5px;
  }

  &__location {
    margin-bottom: 34px;
  }

  &__roomNumber {
    color: #FFFFFF;
    font-size: 28px;
    background-color: $clr_accentcolor;
    border-radius: 10px;
    padding: 15.5px 36px;
    margin-right: 25px;
    font-family: "Fredoka One";
  }

  &__time {
    font-size: 28px;
    padding: 15.5px 0;
    font-family: "Fredoka One";
  }

  &__sessionTitle {
    font-size: 28px;
    font-weight: bold;
    margin-bottom: 20px;
  }

  &__sessionSubTitle {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 35px;
  }

  &__description {
    font-size: 18px;
    font-weight: bold;
  }

  &__hr {
    border: 2px solid $clr_basecolor;
  }

  &__speaker {
    padding-top: 52.5px;
    display: flex;
    flex-wrap: nowrap;
  }

  &__speakerSns {
    text-align: center;
    min-width: 182px;
    margin-right: 80px;
  }

  &__speakerImg {
    width: 182px;
    height: 182px;
    margin-bottom: 20px;
  }

  &__followIcon {
    width: 35px;
    height: 35px;
    margin: 0 13.5px;
  }

  &__speakerName {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 10px;
  }

  &__speakerCompany {
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 18px;
  }
}
</style>
