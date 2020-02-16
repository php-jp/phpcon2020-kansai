<template>
  <nav class="c-share">
    <p class="c-share__text">Share</p>
    <div class="c-share__icons">
      <a
        class="c-share__link"
        href="https://twitter.com/intent/tweet?text=%E9%96%A2%E8%A5%BF%E6%9C%80%E5%A4%A7%E3%81%AEPHP%E3%82%A4%E3%83%99%E3%83%B3%E3%83%88%E3%81%AF5%E6%9C%8809%E6%97%A5(%E5%9C%9F)%E3%81%AB%E3%83%96%E3%83%AA%E3%83%BC%E3%82%BC%E3%83%97%E3%83%A9%E3%82%B6%E3%83%9B%E3%83%BC%E3%83%AB%E3%82%AB%E3%83%B3%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E3%81%AB%E3%81%A6%E9%96%8B%E5%82%AC!%20PHP%E3%82%AB%E3%83%B3%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E9%96%A2%E8%A5%BF2020%20https://2020.kphpug.jp/&hashtags=phpkansai"
      >
        <img
          src="@/assets/images/share/share_icon_twitter.svg"
          class="c-share__icon"
          alt="twitter-icon"
        />
      </a>
      <a
        class="c-share__link"
        href="https://www.facebook.com/sharer.php?u=https://2020.kphpug.jp&t=%E9%96%A2%E8%A5%BF%E6%9C%80%E5%A4%A7%E3%81%AEPHP%E3%82%A4%E3%83%99%E3%83%B3%E3%83%88%E3%81%AF5%E6%9C%8809%E6%97%A5(%E5%9C%9F)%E3%81%AB%E3%83%96%E3%83%AA%E3%83%BC%E3%82%BC%E3%83%97%E3%83%A9%E3%82%B6%E3%83%9B%E3%83%BC%E3%83%AB%E3%82%AB%E3%83%B3%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E3%81%AB%E3%81%A6%E9%96%8B%E5%82%AC!%20PHP%E3%82%AB%E3%83%B3%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E9%96%A2%E8%A5%BF2020&hashtags=phpkansai"
      >
        <img
          src="@/assets/images/share/share_icon_facebook.svg"
          class="c-share__icon"
          alt="facebook-icon"
        />
      </a>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";
.c-share {
  position: fixed;
  z-index: 999;
  margin-top: 110px;
  width: 60px;
  max-width: 60px;
  left: 82px;
  user-select: none;

  @include mobile {
    display: none;
  }

  &__text {
    font-family: "Fredoka One", cursive;
    color: $clr-accentcolor;
    font-size: 30px;
    letter-spacing: 2.1px;
    writing-mode: vertical-rl;

    &:after {
      content: "";
      width: 4px;
      height: 115px;
      background-color: $clr-accentcolor;
      display: inline-block;
      margin-top: 23px;
      margin-bottom: 27px;
    }
  }

  &__icons {
    display: flex;
    flex-direction: column;
  }

  &__link {
    text-align: center;
    &:hover {
      opacity: 0.7;
      transition: 0.3s;
    }
  }
  &__icon {
    margin-top: 14px;
  }
}
</style>
