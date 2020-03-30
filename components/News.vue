<template>
    <section class="p-news">
      <div class="l-container">
        <div class="p-news__title">news</div>
        <div class="p-news__intro">
          <h2 class="p-news__secHeading">新型コロナウィルス感染症に関する対応方針について</h2>
          <p class="p-news__read">
            PHPカンファレンス関西2020 運営委員長の加納悠史です。<br>
            このたび、PHPカンファレンス関西2020運営委員会は、新型コロナウィルス感染症 (COVID-19) の感染拡大を鑑み、2020年5月9日に予定しておりましたPHPカンファレンス関西2020の開催を断念することに決定いたしました。<br>
            楽しみにして頂いた皆様に心よりお詫び申し上げます。<br>
            運営委員会では、感染の拡大状況を注視し、開催について検討を重ねて参りましたが、現段階で開催予定日の5月9日に事態が収束しているとは判断できませんでした。このまま開催を目指したとしても、協賛してくださるスポンサーの皆様や、これから登壇に向けて準備してくださるスピーカーの方々、並びに参加を考えてくださっている方々に不安を与えてしまい、関係者が望む形での開催が難しいと考えたため、今回の決断に至りました。<br>
            今回、すでにご応募頂いておりましたスポンサー、スピーカーの皆様には、追ってご連絡させていただきます。<br>
            また、前述の通り、予定しておりました5月の開催は見送らせていただきますが、運営委員会では、年内の開催を模索し、可能性が見えれば改めて告知させていただきます。<br>
            非常に心苦しい限りですが、何卒、ご理解のほどよろしくお願いいたします。
          </p>
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

.p-news {
  margin: 0 auto ;
  position: relative;
  color: $clr_accentcolor;
  background-color: $clr_basecolor;
  @include desktop {
    background-image:url("~assets/images/about/about_zou_left.png"),url("~assets/images/about/about_zou_right.png");
    background-position: bottom 20px left 6%,bottom 20px right 0px;
    background-repeat: no-repeat;
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
    margin-bottom: 100px;
    @include desktop {
      text-align: center;
      padding: 50px 80px 90px 80px;
      font-size: 2.8rem;
      margin-bottom: 200px;
    }
  }

  &__secHeading {
    display: inline-block;
    text-align: center;
    letter-spacing: 1.12px;
    font-size: 1.6rem;
    margin-bottom: 20px;

    @include desktop {
    height: 39px;
    font-size: 2.8rem;
    margin-bottom: 45px;
    margin-top: 25px;
    }


  }

  &__read {
    display: inline-block;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    font-size: 1.3rem;
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
}

</style>
