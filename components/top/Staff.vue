<template>
    <section class="p-staff">
        <div class="l-container">
            <div class="p-staff__title">organization</div>
            <p class="p-staff__sentenceHead">「関西PHPユーザーズグループ/PHPカンファレンス関西実行委員会」</p>
            <p class="p-staff__sentence">
                関西PHPユーザーズグループは関西を中心に活動するPHPユーザの交流を目的とする団体です。
                <br>
                PHPカンファレンス関西実行委員会はその中からカンファレンス開催を目的として集まった有志メンバーであり、
                <br>
                毎月数回のミーティングを行い、本イベントの開催準備を進めています。
            </p>
            <div class="p-staff__titleSub">staff</div>
            <div class="p-staff__staffWrap">
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                    <img class="p-staff__staffImage" src="~/assets/images/staff/0.png" alt="スタッフ写真">
                    <p class="p-staff__staffName">山田太郎</p>
                </div>
                <div class="p-staff__staff">
                </div>
                <div class="p-staff__staff">
                </div>
                <div class="p-staff__staff">
                </div>
                <div class="p-staff__staff">
                </div>
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

.p-staff {
    position: relative;
    @include desktop {
        padding-bottom: 75px;
    }
    &__title {
        @include c-section-title;
        display: none;
        color: $clr_accentcolor;
        @include desktop {
            display: block;
        }
    }
    &__titleSub {
        @include c-section-title;
        color: $clr_accentcolor;
        @include desktop {
            color: #FFFFFF;
            -webkit-text-stroke: 2px $clr_accentcolor;
            font-size: 35px;
        }
    }
    &__staffWrap {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        width: 280px;
        margin: 0 auto;
        @include desktop {
            width: 100%;
        }
    }
    &__staff {
        margin-bottom: 95px;
        @include desktop {
            width: 16%;
        }
    }
    &__staffImage {
        width: 80px;
    }
    &__staffName {
        color: $clr_accentcolor;
        font-weight: bold;
    }

    &__sentenceHead {
        display: none;
        font-size: 20px;
        color: $clr_accentcolor;
        font-weight: bold;
        text-align: center;
        @include desktop {
            display: block;
        }
    }
    &__sentence {
        display: none;
        font-size: 16px;
        color: $clr_accentcolor;
        text-align: center;
        @include desktop {
            display: block;
        }
    }
}

</style>