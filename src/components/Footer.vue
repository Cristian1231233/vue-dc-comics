<template>
  <footer>
      <section class="footer-top">
       <div class="container">
           <div class="informative">
           <h2>DC COMIX</h2>
           <ul>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
           </ul>
           <h2 class="shop">SHOP</h2>
           <ul>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
           </ul>
           </div>
           <div class="informative">
           <h2>DC</h2>
           <ul>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
           </ul>
           </div>
           <div class="informative">
           <h2>SITES</h2>
           <ul>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
               <li><a href="#">Characters</a></li>
           </ul>
           </div>
            
       </div>
      </section>
      <section class="footer-button">
        <div class="container2">
            <div class="button-social">
                <div class="button">
                  <button>SIGN-UP NOW!</button>
                </div>
                <div class="socials">
                    <h1>FOLLOW US</h1>
                   <div class="social">
                       
                       
                      <img src="../assets/img/footer-facebook.png"
                      alt="">
                   </div>
                   <div class="social">
                      <img src="../assets/img/footer-twitter.png"
                      alt="">
                   </div>
                   <div class="social">
                      <img src="../assets/img/footer-youtube.png"
                      alt="">
                   </div>
                   <div class="social">
                      <img src="../assets/img/footer-pinterest.png"
                      alt="">
                   </div>
                   <div class="social">
                      <img src="../assets/img/footer-periscope.png"
                      alt="">
                   </div>
                </div>
                
            </div>
        </div>
      </section>
      
  </footer>
</template>

<script>
export default {
    nome:'Footer'
}
</script>

<style lang="scss" scoped>


    
    
    .footer-top{
        
        background-image: url('../assets/img/footer-bg.jpg');
       
    }
    .footer-button{
        height: 90px;
        background-color: gray;
    }


.container{
    width: 860px;
    margin: 0 auto;
    display: flex;
    padding-bottom: 30px;

    .informative{
        margin-top: 30px;
        margin-right: 40px;

        ul li{
            list-style: none;
            font-size: 12px;

            a{
                text-decoration: none;
                color: gray;
            }
        }
        h2{
            color: white;
            font-size: 15px;
            
            margin-bottom: 10px;
        }
        .shop{
            margin-top: 10px;
        }
    }
}
.container2{
    width: 860px;
    height: 90px;
    margin: 0 auto;
    display: flex;
    align-items: center;
}

.button-social{
    width: 100%;
    height: 60px;
    border: 1px solid black;
    display: flex;
    align-items: center;
    justify-content: space-between;
    button{
        color: white;
        border: 2px solid blue;
        background-color: gray;
        padding: 10px;
    }
    .socials{
        display: flex;
        align-items: center;
        .social{
            height: 30px;
            margin-left: 10px;
            
            img{
                height: 100%;
                
            }
        }
    }
}


</style>