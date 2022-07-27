<template>
  <div class="col py-large text-center border border-top-0 border-bottom-0">
    <h5 class="fw-bolder">{{ resultData.title }}</h5>
    <span class="d-block number-result py-3"> {{ resultData.num }}</span>
    <span class="d-block fw-bold subtitle-text"> {{ resultData.numInfo}}</span>
  </div>
</template>

<script>
export default {
    props:{
        resultData:Object,
    }
}
</script>

<style lang="scss">
@import "../../styles/variables.scss";
.number-result{
  color:$mainColor;
  font-size: 4rem; 
  font-weight: bolder;
}
</style>