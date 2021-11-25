<template>
  <div class="creat-card">
      <div class="immage">
     <img :src="propImg" :alt="propTitle">
     </div>
     <h3>{{propTitle}}</h3>
  </div>
</template>

<script>
export default {
    nome: 'ProductCard',
    props:{
        propImg: String,
        propTitle: String,
        
    }
}
</script>

<style lang="scss" scoped>

.creat-card{
    width: calc(100% / 6);
    margin-top: 1rem;
    .immage{
        width: 130px;
        height: 130px;
        img{
            width: 100%;
            height: 100%;
        }
    }
    h3{
        font-size: 16px;
        margin-top: 1rem;
        margin-bottom: 2rem;
    }
}

</style>