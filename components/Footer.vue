<template>
<div class="p-footer">
    <div class="square">
      <img class="square_logo" src="~assets/images/footer/footer_icon_logo.svg">
    </div>
    <div class="p-footer_intro">
      <div class="p-footer_secHeading">
        お問い合わせは<a>Facebookグループ</a>のメッセージからお願いします。
      </div>
      <div class="p-footer_read">
        follow me‼︎
      </div>
      <div class="p-footer_follow">
        <img class="p-footer_followIcon" src="~assets/images/footer/footer_icon_facebook.svg" alt="facebook">
        <img class="p-footer_followIcon" src="~assets/images/footer/footer_icon_twitte.svg" alt="twitter">
      </div>
      <p class="p-footer_copyright">
        Copyright @ Kansai PHP Users Group
      </p>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~assets/scss/common.scss";

.square {
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

  &_logo {
    width: 48px;
    height: 38px;
  }
}

.p-footer {
    background-color: #433937;
    color: $clr_accentcolor;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    position: relative;
    padding: 56px 28px 30px 29px;

    &_secHeading {
      font-size: 1.4rem;
      margin-bottom: 22px;

      @include desktop {
        font-size: 2rem;
        margin-bottom: 51px;
      }

      a {
        text-decoration: underline;
      }
    }

    &_read {
        font-size: 1.4rem;
        margin-bottom: 15px;
        letter-spacing: 0.98px;

        @include desktop {
        font-size: 2rem;
         margin-bottom: 25px;
        }
    }

    &_follow {
      display: flex;
      justify-content: center;
      &Icon {
        display: inline-block;
        width: 30px;
        height: 30px;
        &:first-child {
          margin-right: 30px;
        }
      }
    }

    &_copyright {
        font-size: 1.2rem;
        margin-top: 42px;

        @include desktop {
          font-size: 1.5rem;
          margin-bottom: 34px;
        }
    }
}

</style>