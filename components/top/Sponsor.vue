<template>
    <section class="p-sponsor">
        <div class="l-container">
            <div class="p-sponsor__title">
                sponsor
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
    &__title {
        @include c-section-title;
        color: $clr_accentcolor;
        padding: 0;
    margin-bottom: 25px;
    }
}
</style>