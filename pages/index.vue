<template>
  <main>
    <div class="c-background">
      <Share />
      <p-hero></p-hero>
      <p-about></p-about>
      <p-access></p-access>
      <L-footer></L-footer>
    </div>
  </main>
</template>

<script>
import PHero from '~/components/top/Hero.vue'
import PAbout from '~/components/top/About.vue'
import PAccess from '~/components/top/Access.vue'
import Share from "~/components/top/-Share.vue";
import LFooter from "~/components/Footer.vue";

export default {
  components: {
    PHero,
    PAbout,
    PAccess,
    LFooter,
    Share
  },
  head: {
      title: 'PHPカンファレンス関西2020 は 5月9日(土)にグランフロント大阪にて開催!',
      meta: [
        { property: 'og:title', content: 'PHPカンファレンス関西2020 は 5月9日(土)にグランフロント大阪にて開催!' },
        { property: 'og:image', content: 'https://2020.kphpug.jp/images/ogp.jpg' },
        { property: 'og:url', content: 'https://2020.kphpug.jp/' },
        { property: 'og:description', content: '関西PHPerの夏はこれがなくちゃ始まらない！今年で9回目となる関西最大級のPHPイベント、今年も開催です。全国PHPerが大阪に集結「PHPカンファレンス関西」で心に残る夏の思い出を！' },
        { name: 'description', content: '関西PHPerの夏はこれがなくちゃ始まらない！今年で9回目となる関西最大級のPHPイベント、今年も開催です。全国PHPerが大阪に集結「PHPカンファレンス関西」で心に残る夏の思い出を！' }
      ]
    }
}
</script>

<style lang="scss" scoped>

@import "~/assets/scss/common.scss";

.c-background {

  &:before {
    content:"";
    width: 100vw;
    height: 100vh;
    background-image: url('~assets/images/hero/hero_sp_zou.png');
    background-repeat: no-repeat;
    background-size: 100%;
    display: block;
    position: fixed;
  }

    @include desktop(){
    &:before {
      background:none;
    }
}
}
</style>
