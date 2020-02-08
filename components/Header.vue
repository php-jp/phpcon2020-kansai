<template>
  <section class="p-header">
    <h1 class="p-header__image">
      <img class="p-header__image--menu" src="~/assets/images/header/header_icon_hamburger.svg" alt="">
    </h1>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.p-header {
  margin-top: 14px;
  &__image {
    display: flex;
    &--menu {
      margin-left: auto;
      margin-right: 20px;
      width: 46px;
      height: 46px;
      @include desktop {
        width: 100%;
        height: 100%;
      }
    }
  }
}
</style>
