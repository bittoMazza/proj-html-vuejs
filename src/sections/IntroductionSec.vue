<template>
  <section class="py-4">
        <div class="container">
            <div class="d-flex align-items-center my-4">
                <div class="col-5 pe-5">
                    <h2 class="fw-bold bold-text-color">Distant learning for further expansion</h2>
                    <p class="p-text font-normal">Learning is a life-long journey that in fact we nerver finda the terminate stop. Stop searching,enjoy the process.</p>
                    <button class="my-3 main-btn-style"> <i class="bi bi-download"></i> Download free guide </button>
                    <span class="d-block">Have questions? <a href="#" class="underline-main-link fw-bold">Get Free Sample <i class="bi bi-arrow-right"> </i> </a></span>
                </div>
                <div class="col-7 ps-5 position-relative">
                        <img src="../assets/Images/maxcoach-shape-02.png" class="position-absolute bottom-50 end-0 z-index-n1" alt="">
                        <img src="../assets/Images/maxcoach-shape-07-150x150.png"  class="position-absolute bottom-50 start-0 z-index-n1 mb-2" alt="">
                        <img src="../assets/Images/maxcoach-shape-07-150x150.png" class="position-absolute top-50 start-0 z-index-n1 mt-2" alt="">
                        <img src="../assets/Images/maxcoach-shape-07-150x150.png" class="position-absolute bottom-0 start-50 z-index-n1" alt="">
                        <i class="bi bi-circle circle-position circle-bg-image"></i>             
                    <img src="../assets/Images/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" class="ms-5 rounded-circle w-75" alt="">
                </div>
            </div>
            <div class="clients-logo d-flex justify-content-between py-4">
                <div v-for="(client,index) in 6" :key="index" class="d-flex align-items-center">
                    <img :src="getClientImg(index)" alt="">    
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    methods:{
        getClientImg(ind){
            return require('../assets/Images/client_logo/client-logo-0'+(ind+1)+'.png')
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/class.scss";
.circle-position{
    position: absolute;
    left: 8%;
    top: 60%;

}
</style>
