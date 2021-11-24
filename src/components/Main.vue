<template>
  <main>
      <section>
      <div class="container">
     <div>-->Content goes here>--</div>
      </div>
      </section>
      <section>
          <div class="container">
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

main{
    height: 90px;
    .container{
        width: 860px;
        height: 90px;
        margin: 0 auto;
        display: flex;
        align-items: center;
        background-color: red;
    }
}
.info-text{
    min-width: 100px;
    background-color: #008000;
    display: flex;
    align-items: center;
    margin: 20px;
    .icon{
        width: 35px;
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