<template>
  <main>
    <L-header></L-header>
    <p-hero></p-hero>
    <p-about></p-about>
    <p-access></p-access>
    <L-footer></L-footer>
  </main>
</template>

<script>
import LHeader from '~/components/Header.vue'
import PHero from '~/components/top/Hero.vue'
import PAbout from '~/components/top/About.vue'
import PAccess from '~/components/top/Access.vue'
import LFooter from "~/components/Footer.vue";


export default {
  components: {
    LHeader,
    PHero,
    PAbout,
    PAccess,
    LFooter
  }
}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

</style>
