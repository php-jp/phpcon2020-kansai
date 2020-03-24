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
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                gold
            </div>
            <div class="p-sponsor__gold">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                silver
            </div>
            <div class="p-sponsor__silver">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
            </div>

            <div class="p-sponsor__titleSub">
                food＆drink
            </div>
            <div class="p-sponsor__food">
                <img src="~/assets/images/sponsor/0.png" alt="コールドスポンサーの会社">
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
    }
    &__platinum img {
        widows: 280px;
        margin-bottom: 20px;
    }
    &__gold {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
    &__gold img {
        width: 130px;
        margin-bottom: 20px;
    }
    &__silver {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
    &__silver img {
        width: 84px;
        margin-bottom: 15px;
    }
    &__food {
        text-align: center;
    }
    &__food img {
        width: 130px;
    }
}
</style>