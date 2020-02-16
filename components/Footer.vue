<template>
  <section class="p-footer">
    <div class="p-footer__square">
      <img
        class="p-footer__squarLogo"
        src="~assets/images/footer/footer_icon_logo.svg"
      />
    </div>
    <div class="p-footer__intro">
      <div class="p-footer__secHeading">
        お問い合わせは<a
          href="https://www.facebook.com/pcon.kansai/"
          target="branck"
          class="p-footer__link"
          >Facebookグループ</a
        >のメッセージからお願いします。
      </div>
      <div class="p-footer__read">
        follow me‼︎
      </div>
      <div class="p-footer__follow">
        <a
          class="p-footer__link"
          href="https://www.facebook.com/pcon.kansai/"
          target="branck"
        >
          <img
            class="p-footer__followIcon p-footer__iconFacebook"
            src="~assets/images/footer/footer_icon_facebook.svg"
            alt="facebook"
          />
        </a>
        <a
          class="p-footer__link"
          href="https://twitter.com/phpcon_kansai"
          target="branck"
        >
          <img
            class="p-footer__followIcon"
            src="~assets/images/footer/footer_icon_twitte.svg"
            alt="twitter"
          />
        </a>
      </div>
      <small class="p-footer__copyright">
        Copyright @ Kansai PHP Users Group
      </small>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~assets/scss/common.scss";

.p-footer {
  background-color: #433937;
  color: $clr_accentcolor;
  font-family: "M PLUS Rounded 1c", sans-serif;
  font-weight: bold;
  text-align: center;
  position: relative;
  padding: 78px 28px 0 29px;

  &__square {
    // padding: 0px 100px 253px;
    padding-top: 14px;
    display: inline-block;
    position: absolute;
    background-repeat: no-repeat;
    width: 120px;
    height: 55px;
    top: 0;
    left: 50%;
    transform: translateX(-50%) translateY(-70%);
    background-color: #433937;
    border-radius: 10px 10px 10px 10px;
    @include desktop {
      width: 370px;
      height: 86px;
    }

    &Logo {
      width: 46px;
      height: 37px;
      @include desktop {
        width: 100px;
        height: 58px;
      }
    }
  }

  &__secHeading {
    font-size: 1.4rem;
    margin-bottom: 22px;

    @include desktop {
      font-size: 2rem;
      margin-bottom: 31px;
    }
  }

  &__link {
    text-decoration: underline;
  }

  &__read {
    font-size: 1.4rem;
    margin-bottom: 15px;
    letter-spacing: 0.98px;

    @include desktop {
      font-size: 2rem;
      margin-bottom: 13px;
    }
  }

  &__follow {
    display: flex;
    justify-content: center;

    &Icon {
      display: inline-block;
      @include mobile {
        width: 30px;
      }
    }

    &__link {
      text-align: center;
    }
  }

  &__iconFacebook {
    margin-right: 30px;
    @include mobile {
      margin-right: 20px;
    }
  }

  &__copyright {
    font-size: 1.2rem;
    margin-top: 49px;
    margin-bottom: 25px;
    font-family: "Fredoka One", cursive;
    font-weight: normal;
    display: inline-block;

    @include desktop {
      font-size: 1.5rem;
      margin-bottom: 30px;
    }
  }
}
</style>
