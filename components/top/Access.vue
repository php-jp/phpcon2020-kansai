<template>
  <section>
    <div class="p-access">
      <div class="c-container">
        <div class="p-access_title">access</div>
        <div class="p-access_flex">
          <div class="p-access_map">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3280.2594918859613!2d135.49170741523224!3d34.69863438043504!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6000e68cd2b0df55%3A0x349166def7ac6e94!2z6LK444GX5Lya6K2w5a6kIOaiheeUsCDjg5bjg6rjg7zjgrzjg5fjg6njgrYg5aSn6Ziq!5e0!3m2!1sja!2sjp!4v1581060142325!5m2!1sja!2sjp" width="100%" height="100%" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
          </div>
          <div class="p-access_how">
            <div class="p-access_place">
              <p class="p-access_text">会場：ブリーゼプラザ ホール & カンファレンス</p>
              <p class="p-access_text">住所：〒530-0001　大阪市北区梅田2-4-9</p>
              <p class="p-access_text">&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;ブリーゼタワー7-8階</p>
            </div>
            <div class="p-access_content">
              <p class="p-access_text">電車でのアクセス</p>
            </div>
            <div class="p-access_intro">
              <p class="p-access_text">四つ橋線西梅田駅より徒歩3分</p>
              <p class="p-access_text">阪神梅田駅（西改札）より徒歩5分</p>
              <p class="p-access_text">JR大阪駅（桜橋口）より徒歩5分</p>
              <p class="p-access_text">JR東西線北新地駅より徒歩5分</p>
            </div>
            <div class="p-access_button">
              <a class="p-googlemap" onclick="location.href='https://g.page/breeze-plaza?share'">Google Mapを見る</a>
            </div>
          </div>
        </div>
      </div>
      </div>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-access {
  margin: 50px auto 0;
  position: relative;
  // background-image:
  //         url("~assets/img/about_frame01.png"),
  //         url("~assets/img/about_frame02.png");
  // background　: $clr_basecolor;
  background-size: 15%, 15%, 30%, 30%;
  background-position: left top, right bottom, 45% 0%, 50% 100%;

  @include desktop {
    margin-top: 100px;
    background-size: 15%, 15%, 15%, 18%;
    background　: $clr_basecolor;
    margin: 90px auto 0;
    height: 800px;
  }

  &_title {
    @include c-section-title;
    color: $clr_accentcolor;
    padding: 0;
    margin-bottom: 25px;
  }

  &_flex {
    display: flex;
    flex-direction: column;
    align-items: center;
    @include desktop {
      flex-direction: row;
      justify-content: center;
      align-items:unset;
    }
  }

  &_how {
    @include desktop {
      display:inline;
    }
  }

  &_text {
    font-size: 13px;
  }

  &_place {
    text-align: left;
    margin-bottom: 23px;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    color: $clr_accentcolor;
    @include desktop {
      font-size: 1.6rem;
    }
  }

  &_map {
    width: 280px;
    height: 200px;
    margin-bottom: 16px;
    @include desktop {
      padding-right: 86px;
      width: 426px;
      height: 300px;
      margin-bottom: unset;
    }
  }

  &_content {
    text-align: left;
    margin-bottom: 8px;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    font-size: 1.6em;
    color: $clr_accentcolor;
  }

  &_intro {
    text-align: left;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    font-size: 1.6rem;
    color: $clr_accentcolor;
    margin-bottom: 25px;
    @include desktop {
      margin-bottom: 20px;
    }
  }

  &_button {
    margin-bottom: 109px;
    text-align: center;
    @include desktop {
      margin-bottom: unset;
    }
  }
}

.p-googlemap {
  width:260px;
  height:50px;
  font-size: 20px;
  padding: 6px;
  display: block;
  background: $clr_accentcolor;
  font-family: 'M PLUS Rounded 1c', sans-serif;
  border-radius: 10px;
  font-weight: bold;
  color: #ffffff;
}

iframe {
  display: inline;
}



</style>
