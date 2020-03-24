<template>
    <section class="p-sheresns">
        <div class="l-container">
            <div class="p-sheresns__title">Share on SNS</div>
            <p class="p-sheresns__sentence">
                ワクワクをシェアしよう！
                <br>
                イベントに関する要望等もお待ちしております。
            </p>
            <div class="p-sheresns__buttons">
                <a
                    class="p-sheresns__link"
                    href=""
                    target="branck"
                >
                    <img src="~/assets/images/sharesns/twitter-brands.svg" alt="">
                    Twiiterでつぶやく
                </a>
                <a
                    class="p-sheresns__link"
                    href=""
                    target="branck"
                >
                    <img src="~/assets/images/sharesns/facebook-f-brands.svg" alt="">
                    Facebookでシェア
                </a>
            </div>

            <p class="p-sheresns__sentence">
                みんなの様子を覗いてみよう！
            </p>

            <a class="p-sheresns__tag" href="" target="_blanck">
                #phpkansai
            </a>
        </div>
    </section>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-sheresns {
    margin: 0 auto ;
    padding-bottom: 86px;
    position: relative;
    color: $clr_accentcolor;
    background-color: $clr_basecolor;
    @include desktop() {
        padding-bottom: 170px;
    }

    &__title {
        @include c-section-title;
        @include desktop() {
            padding-bottom: 52px;
        }
    }
    &__sentence {
        text-align: center;
        font-size: 12px;
        font-weight: bold;
        padding-bottom: 17px;
        @include desktop() {
            padding-bottom: 31px;
            font-size: 18px;
        }
    }

    &__buttons {
        margin-bottom: 33px;
        @include desktop() {
            width: 590px;
            display: flex;
            justify-content: space-between;
            margin: 0 auto 52px;
        }
    }

    &__link {
        width: 260px;
        height: 50px;
        font-size: 18px;
        display: flex;
        justify-content: center;
        align-items: center;
        background: $clr_accentcolor;
        font-family: "M PLUS Rounded 1c", sans-serif;
        border-radius: 10px;
        font-weight: bold;
        color: #ffffff;
        text-decoration: none;
        margin: 0 auto 15px;
        @include desktop() {
            width: 280px;
            height: 60px;
            margin: 0
        }
    }
    &__link img {
        height: 15px;
        margin-right: 12px;
    }

    &__tag {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 200px;
        height: 40px;
        background-color: #fff;
        margin: 0 auto;
        border-radius: 30px;
        text-decoration: none;
        font-weight: bold;
        @include desktop() {
            width: 280px;
            height: 60px;
        }
    }
}

</style>