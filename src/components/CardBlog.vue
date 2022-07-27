<template>
<div class="card mx-3">
  <img class="card-img-top" :src="getCardImg()" alt="Card image cap">
  <div>
    <span>{{blog.type}}</span>
  </div>
  <div class="card-body">
    <h4 class="card-text">{{blog.title}}</h4>
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
            return require('../assets/Images/'+this.blog.image+'')
        }
    }
}
</script>

<style>
</style>