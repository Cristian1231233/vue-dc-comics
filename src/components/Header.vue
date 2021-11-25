<template>
  <header>
      <div class="container">
      <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu-link">
          <nav>
              <ul>
                  <li v-for="(item, index) in links" :key="index"
                  ><a :class="{active: item.current}" :href="item.url"><strong>{{item.text}}</strong>
                  </a>
                  <div class="line"></div>
                  </li>
              </ul>
          </nav>
      </div>
      </div>
  </header>
</template>

<script>
export default {
    nome: 'Header',
    data(){
        return{
           
            links:[
                {
                    url: '/',
                    text: 'CHARACTERS',
                    current: false
                },
                {
                    url: '/',
                    text: 'COMIX',
                    current: true
                },
                {
                    url: '/',
                    text: 'MOVIES',
                    current: false
                },
                {
                    url: '/',
                    text: 'TV',
                    current: false
                },
                {
                    url: '/',
                    text: 'GAMES',
                    current: false
                },
                {
                    url: '/',
                    text: 'COLLECTIBLES',
                    current: false
                },
                {
                    url: '/',
                    text: 'VIDEOS',
                    current: false
                },
                {
                    url: '/',
                    text: 'FANS',
                    current: false
                },
                {
                    url: '/',
                    text: 'NEWS',
                    current: false
                },
                {
                    url: '/',
                    text: 'SHOP',
                    current: false
                }


            ]
        }
    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/mixin.scss';



header{
    height: 90px;
    @include flex(a);
    
    .container{
        @include flex(ja);
        width: 860px;
        height: 90px;
        margin: 0 auto;
        .logo{
            width: 70px;
            img{
                width: 100%;
                height: 100%;
            }
        }
    }
    
    .active{
        color: $colore-blu;
    }
    nav ul{
        display: flex;
        li{
            list-style: none;
            height: 90px;
            line-height: 90px;
           
            
            
            a{
                color: black;
                text-decoration: none;
                font-size: 11px;
                padding: 0.3rem;
                width: 100%;
                height: 100%;
                &:hover{
                    color: $colore-blu;
                }
            }
        }
    }
}

</style>