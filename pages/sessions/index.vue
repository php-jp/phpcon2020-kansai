<template>
  <main>
    <PSessions />
    <Sharesns />
    <L-footer></L-footer>
  </main>
</template>

<script>
import Share from "~/components/top/-Share.vue";
import Sharesns from "~/components/top/Sharesns.vue"
import LFooter from "~/components/Footer.vue";
import PSessions from "~/components/Sessions.vue"

export default {
  components: {
    LFooter,
    Share,
    Sharesns,
    PSessions
  },
  head: {
    title: 'PHPカンファレンス関西2020 は 5月9日(土)に開催!',
    meta: [
      { property: 'og:title', content: 'PHPカンファレンス関西2020 は 5月9日(土)に開催!' },
      { property: 'og:image', content: 'https://2020.kphpug.jp/images/ogp.jpg' },
      { property: 'og:url', content: 'https://2020.kphpug.jp/' },
      { property: 'og:description', content: '集え、PHPer！！PHPerのGWはこの日が本番あのPHPの祭典がついに帰ってきた！今回のテーマは「Share!!」当日はPHPに関するトークセッションのほか、懇親会やその他イベントを実施予定「PHPカンファレンス関西」で知識•技術•感動をみんなで分かち合おう！' },
      { name: 'twitter:card', content: 'summary_large_image' },
      { name: 'description', content: '集え、PHPer！！PHPerのGWはこの日が本番あのPHPの祭典がついに帰ってきた！今回のテーマは「Share!!」当日はPHPに関するトークセッションのほか、懇親会やその他イベントを実施予定「PHPカンファレンス関西」で知識•技術•感動をみんなで分かち合おう！' }

    ]
  }
}
</script>
