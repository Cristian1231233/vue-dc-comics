<template>
  <main>
      <section class="black">
          <button class="carica move">CURRENT SERIES</button>
          <section class="jumbotron">
          </section>
          <section class="main-buttom">
            <div class="container">
                 <ProductCard v-for="(serie, index) in seriesCartoons" :key="index" 
                 :propImg="serie.thumb" 
                 :propTitle="serie.series"
                 />
                <div class="Load">
                    <button class="carica">Load more</button>
                </div>
                 
                 
           </div>
         </section>
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

import ProductCard from './ProductCard';

export default {
    nome:'Main',
    components: {
        ProductCard
    },
    data(){
        return {
            seriesCartoons: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]
        }
    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/mixin.scss';


main{
    section.black{
        color: white;
        background-color: black;
        position: relative;
        .move{
            position: absolute;
            top: 284px;
            left: 220px;
            height: 30px;
        }
    }
    section.jumbotron{
        height: 300px;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: 1500px;
        
    }
    section.blu{
        color: rgba(248, 228, 228, 0.966);
        background-color: $colore-blu;
    }
    section.main-buttom{
        background-color: #1C1C1C;
        
    }
    
    .container{
        width: 860px;
        min-height: 300px;
        margin: 0 auto;
        padding: 10px;
        display: flex;
        flex-wrap: wrap;
        .Load{
            width: 100%;
            text-align: center;
            
        }
    }
    .container-2-main{
        width: 860px;
        height: 90px;
        margin: 0 auto;
        @include flex(a);
    }
}
.carica{
      width: 150px;
      height: 20px;
      color: white;
      background-color: $colore-blu;
      border: none;
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