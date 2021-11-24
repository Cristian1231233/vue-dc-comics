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
                  ><a :href="item.url"><strong>{{item.text}}</strong></a></li>
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
                    current: 'true'
                },
                {
                    url: '/',
                    text: 'COMIX',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'MOVIES',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'TV',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'GAMES',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'COLLECTIBLES',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'VIDEOS',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'FANS',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'NEWS',
                    current: 'false'
                },
                {
                    url: '/',
                    text: 'SHOP',
                    current: 'false'
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
    nav ul{
        display: flex;
        li{
            list-style: none;
            a{
                color: black;
                text-decoration: none;
                font-size: 11px;
                padding: 0.3rem;
                &:hover{
                    color: $colore-blu;
                }
            }
        }
    }
}

</style>