<template>
  <div class="col-4 px-3">
    <img class="" :src="getCardImg()" alt="">
    <h6 class="pt-4"> {{ cardBenefit.title }} </h6>
    <p class="py-1"> {{ cardBenefit.info }}</p>
    <a href="#" class="fw-bold"> {{cardBenefit.linkText}} <i class="bi bi-arrow-right"></i> </a>
  </div>
</template>

<script>
export default {
    props:{
        cardBenefit:Object
    },
    methods:{
        getCardImg(){
            return require('../../assets/Images/'+this.cardBenefit.image+'')
        }
    }
}
</script>

<style lang="scss">
@import "../../styles/variables.scss";
</style>