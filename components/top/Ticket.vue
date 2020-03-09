
<template>
  <section>
    <div class="p-ticket">
      <div class="l-container" >
        <div class="p-ticket_title">ticket</div>
          <p class="p-ticket_read">
            FRONTEND CONFERENCE 2019 の参加にはチケットの購入が必要です。<br>
            チケットの購入は Peatix にて<br>
          </p>
          <div class="p-ticket__button">
          <a href="" target ="_blank" >Peatixへ</a>
          </div>
        </div>
      </div>
    
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";
 $font-family:"M PLUS Rounded 1c";


.p-ticket {
  position: relative;
  color: $clr_accentcolor;
  background-color: #FFFAF8;
  text-align: center;

  &_title {
    @include c-section-title;
  }
  &_read {
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;
    font-size: 1.8rem;
    line-height: 3;
    @include desktop {
    display: inline-block;
    color: #F29B85;
    text-align: center;
    font-size: 1.8rem;
    line-height: 2;
    }
  }

  &__button {
  box-sizing: border-box;
  text-decoration: none;
  font-size: 1.8rem;
  color:#fff;
  font-weight: bold;
  line-height: 1.4;
  padding: 10px 0px 10px 10px;
  background-color: $clr-accentcolor;
  border-radius: 10px 9px 9px 10px;
  margin: 0 auto;
  &:nth-child(1) {
    margin-right: 20px;
    @include desktop {
      margin-right: 40px;
    }
  }
  @include desktop {
    text-align: center;
    margin-top: 55px;
    width:260px;
    font-size: 20px;
  }
}

   
}
</style>