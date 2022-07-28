<template>
<div class="card shadow-card">
  <img class="card-img-top" :src="getCardImg()" alt="Card image cap">
  <div class="px-4 py-4">
    <span class="subtitle-text">{{blog.type}}</span>
    <h5 class="card-text py-2 lh-base">{{blog.title}}</h5>
     <div>
      <span class="pe-5 small-text-color"><i class="bi bi-calendar pe-1"></i> {{blog.lastUpdate}}</span>
      <span class="small-text-color"><i class="bi bi-eye pe-1"></i> {{blog.view}} view</span>
    </div>
  </div> 
</div>
</template>

<script>
export default {
    props:{
        blog:Object,
    },
    methods:{
        getCardImg(){
            return require('../../assets/Images/'+this.blog.image+'')
        }
    }
}
</script>

<style lang="scss">
@import "../../styles/variables.scss";
@import "../../styles/class.scss";
.shadow-card{
  box-shadow: 0 5px 20px 5px rgb(232, 232, 232);
}
</style>