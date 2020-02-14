<template>
  <main>
    <div class="c-background">
      <p-hero></p-hero>
      <p-about></p-about>
      <p-access></p-access>
      <L-footer></L-footer>
    </div>
  </main>
</template>

<script>
import PHero from '~/components/top/Hero.vue'
import PAbout from '~/components/top/About.vue'
import PAccess from '~/components/top/Access.vue'
import LFooter from "~/components/Footer.vue";


export default {
  components: {
    PHero,
    PAbout,
    PAccess,
    LFooter
  }
}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.c-background {
    background-image: url('~assets/images/hero/hero_sp_zou.png');
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-size: 100%;
    @include desktop(){
      background-image: url("");
    }
}

</style>
