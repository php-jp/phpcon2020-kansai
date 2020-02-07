<template>
<div class="p-footer">
    <div class="square"></div>
        <div class="p-footer_intro">
          <div class="p-footer_secHeading">
            お問い合わせは<a>Facebookグループ</a>のメッセージからお願いします。
          </div>
          <div class="p-footer_read">
            follow me‼︎
          </div>
          <p class="p-footer_copyright">
            Copyright @ Kansai PHP Users Group
          </p>
        </div>
     </div>
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~/assets/scss/common.scss";

.square {
padding: 0px 100px 253px 100px;
   width: 120px;
   height: 55px;
   background: #433937;
   border-radius: 10px 10px 10px 10px; 
   @include desktop {
    width: 370px;
   height: 86px;
        }
}

.p-footer {
    background-color: #433937;
    color: $clr_accentcolor;
    font-family: 'M PLUS Rounded 1c', sans-serif;
    font-weight: bold;
    text-align: center;

    &_secHeading {
        font-size: 1.4rem;
         margin-bottom: 22px;

        @include desktop {
        font-size: 2rem;
         margin-bottom: 51px;
        }
    }

    &_read {
        font-size: 1.4rem;
         margin-bottom: 15px;

        @include desktop {
        font-size: 2rem;
         margin-bottom: 25px;
        }
    }

    &_copyright {
        font-size: 1.2rem;
         margin-bottom: 30px;

        @include desktop {
        font-size: 1.5rem;
         margin-bottom: 34px;
        }
    }
}

</style>