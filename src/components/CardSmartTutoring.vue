<template>
  <div class="col-4 px-3">
    <img class="" :src="getCardImg()" alt="">
    <h6> {{ cardBenefit.title }} </h6>
    <p> {{ cardBenefit.info }}</p>
    <a href="#"> {{cardBenefit.linkText}} --> </a>
  </div>
</template>

<script>
export default {
    props:{
        cardBenefit:Object
    },
    methods:{
        getCardImg(){
            return require('../assets/Images/'+this.cardBenefit.image+'')
        }
    }
}
</script>

<style>

</style>