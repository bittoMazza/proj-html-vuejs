<template>
  <div class="col-4 px-3">
    <img class="" :src="getCardImg()" alt="">
    <span class="pt-4 d-block fs-5 fw-bold bold-text-color"> {{ cardBenefit.title }} </span>
    <p class="py-1 p-text"> {{ cardBenefit.info }}</p>
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
@import "../../styles/class.scss";
</style>