<template>
<div class="card">
  <img class="card-img-top" :src="getCardImg()" alt="Card image cap">
  <div class="px-4 py-3">
    <span>{{blog.type}}</span>
    <h5 class="card-text py-3">{{blog.title}}</h5>
     <div>
      <span class="pe-5"><i class="bi bi-calendar"></i> {{blog.lastUpdate}}</span>
      <span><i class="bi bi-eye"></i> {{blog.view}} view</span>
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

</style>