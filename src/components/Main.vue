<template>
  <main>
      <section class="black">
      <div class="container">
     <div>-->Content goes here>--</div>
      </div>
      </section>
      <section class="blu">
          <div class="container-2-main">
            <div class="info-text">
              <div class="icon">
                 <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              </div>
              <div class="text">DIGITAL COMICS</div>
            </div>
            <div class="info-text">
              <div class="icon">
                 <img src="../assets/img/buy-comics-merchandise.png" alt="">
              </div>
              <div class="text">DC MERCHANDISE</div>
            </div>
            <div class="info-text">
              <div class="icon">
                 <img src="../assets/img/buy-comics-subscriptions.png" alt="">
              </div>
              <div class="text">SUBSCRIPTIONS</div>
            </div>
            <div class="info-text">
              <div class="icon">
                 <img src="../assets/img/buy-comics-shop-locator.png" alt="">
              </div>
              <div class="text">COMIC SHOP LOCATOR</div>
            </div>
            <div class="info-text">
              <div class="icon">
                 <img src="../assets/img/buy-dc-power-visa.svg" alt="">
              </div>
              <div class="text">DC POWER VISA</div>
            </div>
        </div>
      </section>
  </main>
</template>

<script>
export default {
    nome:'Main'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/mixin.scss';


main{
    section.black{
        background-color: black;
        color: white;
    }
    section.blu{
        background-color: $colore-blu;
    }
    
    .container{
        width: 860px;
        height: 90px;
        margin: 0 auto;
        @include flex(a);
    }
    .container-2-main{
        width: 860px;
        height: 90px;
        margin: 0 auto;
        @include flex(a);
    }
}
.info-text{
    min-width: 100px;
    @include flex(a);
    margin: 20px;
    .icon{
        width: 33px;
        height: 38px;
        img{
            width: 100%;
            height: 100%;
        }
        
    }
    .text{
        font-size: 10px;
        margin-left: 10px;
    }
}

</style>