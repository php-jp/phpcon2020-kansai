<template>
    <section class="p-access">
      <div class="l-container">
        <div class="p-access__title">access</div>
        <div class="p-access__flex">
          <div class="p-access__map">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3280.2594918859613!2d135.49170741523224!3d34.69863438043504!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6000e68cd2b0df55%3A0x349166def7ac6e94!2z6LK444GX5Lya6K2w5a6kIOaiheeUsCDjg5bjg6rjg7zjgrzjg5fjg6njgrYg5aSn6Ziq!5e0!3m2!1sja!2sjp!4v1581060142325!5m2!1sja!2sjp"
              width="100%"
              height="100%"
              class="p-access__frame"
              frameborder="0"
              style="border:0;"
              allowfullscreen=""
            ></iframe>
          </div>
          <div class="p-access__how">
            <div class="p-access__lace">
              <p class="p-access__text">
                会場：ブリーゼプラザ ホール & カンファレンス
              </p>
              <p class="p-access__text">
                住所：〒530-0001　大阪市北区梅田2-4-9
              </p>
              <p class="p-access__text">
                &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;ブリーゼタワー7-8階
              </p>
            </div>
            <div class="p-access__content">
              <p class="p-access__text">電車でのアクセス</p>
            </div>
            <div class="p-access__intro">
              <p class="p-access__text">四つ橋線西梅田駅より徒歩3分</p>
              <p class="p-access__text">阪神梅田駅（西改札）より徒歩5分</p>
              <p class="p-access__text">JR大阪駅（桜橋口）より徒歩5分</p>
              <p class="p-access__text">JR東西線北新地駅より徒歩5分</p>
            </div>
            <div class="p-access__button">
              <a
                class="p-access__link"
                href="https://www.google.com/maps/place/%E3%80%92530-0001+%E5%A4%A7%E9%98%AA%E5%BA%9C%E5%A4%A7%E9%98%AA%E5%B8%82%E5%8C%97%E5%8C%BA%E6%A2%85%E7%94%B0%EF%BC%92%E4%B8%81%E7%9B%AE%EF%BC%94%E2%88%92%EF%BC%99+%E3%83%96%E3%83%AA%E3%83%BC%E3%82%BC%E3%82%BF%E3%83%AF%E3%83%BC7-8%E9%9A%8E+%E8%B2%B8%E3%81%97%E4%BC%9A%E8%AD%B0%E5%AE%A4+%E6%A2%85%E7%94%B0+%E3%83%96%E3%83%AA%E3%83%BC%E3%82%BC%E3%83%97%E3%83%A9%E3%82%B6+%E5%A4%A7%E9%98%AA/@34.6987149,135.4939563,13z/data=!4m2!3m1!1s0x6000e68cd2b0df55:0x349166def7ac6e94"
                target="branck"
                >Google Mapを見る</a
              >
            </div>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-access {
  margin: 50px auto 0;
  position: relative;

  @include desktop {
    margin-top: 0;
    margin: 0px auto 0;

    &:before {
      content: "";
      width: 40vw;
      height: 36vw;
      max-width: 527px;
      max-height: 423px;
      background-image: url("../../assets/images/access/access_zou_right.svg");
      background-size: cover;
      background-repeat: no-repeat;
      display: inline-block;
      z-index: -2;
      position: absolute;
      bottom: 8%;
      left: 7%;
    }

    &:after {
      content: "";
      width: 20vw;
      height: 20vw;
      max-width: 322px;
      max-height: 300px;
      background-image: url("../../assets/images/access/access_zou_left.svg");
      background-size: contain;
      background-repeat: no-repeat;
      display: inline-block;
      z-index: -2;
      position: absolute;
      right: 8%;
      bottom: 3%;
    }
  }

  &__title {
    @include c-section-title;
    color: $clr_accentcolor;
    padding: 0;
    margin-bottom: 25px;
  }

  &__flex {
    display: flex;
    flex-direction: column;
    align-items: center;
    @include desktop {
      flex-direction: row;
      justify-content: center;
      align-items: unset;
    }
  }

  &__how {
    @include desktop {
      display: inline;
    }
  }

  &__text {
    font-size: 1.3rem;
    font-weight: bold;
    color: $clr_accentcolor;

    @include desktop {
      font-size: 1.6rem;
    }
  }

  &__frame {
    display: inline;
  }
  &__place {
    text-align: left;
    margin-bottom: 23px;
    font-family: "M PLUS Rounded 1c", sans-serif;
    font-weight: bold;
    color: $clr_accentcolor;
    @include desktop {
      font-size: 1.6rem;
    }
  }

  &__map {
    width: 280px;
    height: 200px;
    margin-bottom: 16px;
    @include desktop {
      padding-right: 50px;
      width: 500px;
      height: 360px;
      margin-bottom: unset;
    }
  }

  &__content {
    text-align: left;
    margin-bottom: 8px;
    font-family: "M PLUS Rounded 1c", sans-serif;
    font-weight: bold;
    font-size: 1.6em;
    color: $clr_accentcolor;
  }

  &__intro {
    text-align: left;
    font-family: "M PLUS Rounded 1c", sans-serif;
    font-weight: bold;
    font-size: 1.6rem;
    color: $clr_accentcolor;
    margin-bottom: 25px;
    @include desktop {
      margin-bottom: 20px;
    }
  }

  &__button {
    margin-bottom: 109px;
    text-align: center;
    @include desktop {
      margin-bottom: 280px;
    }
  }

  &__link {
    width: 260px;
    height: 50px;
    font-size: 18px;
    padding-top: 9px;
    display: block;
    background: $clr_accentcolor;
    font-family: "M PLUS Rounded 1c", sans-serif;
    border-radius: 10px;
    font-weight: bold;
    color: #ffffff;
    text-decoration: none;
    margin: auto;
    @include desktop {
      margin-bottom: 280px;
      margin: 0px;
    }
  }
}
</style>
