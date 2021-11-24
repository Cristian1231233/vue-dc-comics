<template>
  <header>
      <div class="container">
      <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu-link">
          <nav>
              <ul>
                  <li><a href="#">CHARACTERS</a></li>
                  <li><a href="#">COMIX</a></li>
                  <li><a href="#">MOVIES</a></li>
                  <li><a href="#">TV</a></li>
                  <li><a href="#">GAMES</a></li>
                  <li><a href="#">COLLECTIBLES</a></li>
                  <li><a href="#">VIDEOS</a></li>
                  <li><a href="#">FANS</a></li>
                  <li><a href="#">NEWS</a></li>
                  <li><a href="#">SHOP</a></li>
              </ul>
          </nav>
      </div>
      </div>
  </header>
</template>

<script>
export default {
    nome: 'Header'
}
</script>

<style lang="scss" scoped>

header{
    height: 90px;
    display: flex;
    align-items: center;
    background-color: grey;
    
    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        background-color: green;
        width: 860px;
        height: 90px;
        margin: 0 auto;
        .logo{
            width: 70px;
            background-color: blue;
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
            }
        }
    }
}

</style>