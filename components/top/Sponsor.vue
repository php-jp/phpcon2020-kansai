<template>
    <section class="p-sponsor">
        <div class="l-container">
            <div class="p-sponsor__title">
                sponsor
            </div>
            <div class="p-sponsor__titleSub">
                platinum
            </div>
            <div class="p-sponsor__platinum">
                <img src="~/assets/images/sponsor/platinum@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/platinum@2x.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                gold
            </div>
            <div class="p-sponsor__gold">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                silver
            </div>
            <div class="p-sponsor__silver">
                <img src="~/assets/images/sponsor/silver@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/silver@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/silver@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/silver@2x.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/silver@2x.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                food＆drink
            </div>
            <div class="p-sponsor__food">
                <img src="~/assets/images/sponsor/gold@2x.png" alt="コールドスポンサーの会社">
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

.p-sponsor {
    margin: 0 auto ;
    position: relative;
    color: $clr_accentcolor;
    background-color: $clr_basecolor;
    padding: 40px 0 80px;
    @include desktop {
        padding-bottom: 212px;
    }
    &__title {
        @include c-section-title;
        color: $clr_accentcolor;
        padding: 0;
        margin-bottom: 25px;
    }
    &__titleSub {
        text-align: center;
        font-family: 'Fredoka One';
        font-size: 20px;
        margin-bottom: 25px;

        color: #FFFFFF;
        -webkit-text-stroke: 2px $clr_accentcolor;
    }
    &__platinum {
        text-align: center;
        letter-spacing: -.4em;
    }
    &__platinum img {
        letter-spacing: normal;
        width: 280px;
        margin: 0 0 20px;
        @include desktop {
            width: 435px;
            margin: 0 10px 70px;
        }
    }
    &__gold {
        text-align: center;
        letter-spacing: -.4em;
    }
    &__gold img {
        letter-spacing: normal;
        width: 130px;
        margin: 0 10px 20px;
        @include desktop {
            width: 280px;
            margin: 0 15px 50px;
        }
    }
    &__silver {
        text-align: center;
        letter-spacing: -.4em;
    }
    &__silver img {
        letter-spacing: normal;
        width: 84px;
        margin: 0 7.5px 15px;
        @include desktop {
            width: 194px;
            margin: 0 20px 55px;
        }
    }
    &__food {
        text-align: center;
    }
    &__food img {
        width: 130px;
        @include desktop {
            width: 280px;
        }
    }
}
</style>
