<template>
  <div class="col py-5 text-center border border-top-0 border-bottom-0">
    <h6>{{ resultData.title }}</h6>
    <span class="d-block"> {{ resultData.num }}</span>
    <span class="d-block"> {{ resultData.numInfo}}</span>
  </div>
</template>

<script>
export default {
    props:{
        resultData:Object,
    }
}
</script>

<style>

</style>