<template>
    <section class="p-sponsor">
      <div class="l-container">
        <div class="p-sponsor__title">sponsor</div>
        <div class="p-sponsor__square">
          <h2 class="p-sponsor__secHeading">platinum</h2>
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
  @include desktop {
    background-position: bottom 20px left 6%,bottom 20px right 0px;
    background-repeat: no-repeat;
  }

  &__title {
    @include c-section-title;

  }

  &__square {
      background-color: #ffffff;
    border-radius: 10px;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    @include desktop {
      width: 100px;
      height: 100px;
      border-radius: 0px;
      
    }
    display: inline-block;
    width: 100%;
    text-align: center;
    margin-bottom: 35px;
    @include desktop {
      text-align: center;
      padding: 50px 80px 90px 80px;
      font-size: 2.8rem;
      margin-bottom: 100px;
    }
  }

  &__secHeading {
    display: inline-block;
    text-align: center;
    letter-spacing: 1.12px;
    font-size: 1.6rem;
    margin-bottom: 20px;
    font-family: Fredoka One;
    font-weight: bold;

    @include desktop {
         width: 434px;
         height: 39px;
         font-size: 3.5rem;
         margin-bottom: 45px;
         color: #fff;
        -webkit-text-stroke: 1px $clr_accentcolor;
        text-stroke: 1px $clr_accentcolor;
    }


  }

}

</style>
