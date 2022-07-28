<template>
  <section class="py-5 smart-tutoring-section">
        <div class="container px-5">
            <div class="text-center">
                <span class="subtitle-text"> GREAT WORDS ABOUT MAXCOACH </span>
                <span class="h3 fw-bold d-block bold-text-color"> Access <span class="fw-normal main-color-text"> Smart Tutoring </span> Program For Benefits </span>
            </div>
            <div class="d-flex py-5">
                <CardSmartTutoring v-for="(benefit,index) in tutoringBenefits" :key="index"
                :cardBenefit="benefit"
                />
            </div>
            <div class="py-large d-flex align-items-center"> 
                <div class="col-8">
                    <div class="position-relative start-0 w-75">
                        <img src="../assets/Images/maxcoach-shape-07-100x100.png" class="position-absolute top-100 end-0 " alt="">
                        <img class="bottom-shadow w-100" src="../assets/Images/home-2-popup-video-poster.jpg" alt=""> 
                        <img class="youtube-logo" src="../assets/Images/icon-youtube-play.png" alt="">
                    </div>                               
                </div>
                <div class="col-4 pe-5">
                    <span class="subtitle-text">GET STARTED <span class="fw-bold">EFFORTLESSLY</span></span>
                    <span class="h2 fw-bold bold-text-color d-block mt-3">Enjoy Our <span class="fw-normal main-color-text">Companionship</span></span>
                    <p class="py-4 p-text">Learning is a life-long journey that in fact we nerver finda the terminate stop. Stop searching,enjoy the process.</p>
                    <a href="#" class="underline-main-link">Download the guidebook <i class="bi bi-arrow-right"></i></a>
                </div>   
            </div>          
        </div>
    </section>
</template>

<script>
import CardSmartTutoring from './cards/CardSmartTutoring.vue'
export default {
    components:{
        CardSmartTutoring,
    },
    data:function(){
        return{
             tutoringBenefits:[
                {
                    image:'home-2-image-box-01.png',
                    title:'Customize Prefences',
                    info:'You can store online lessons via online cloud or download to your device and revise lessons on the way.',
                    linkText:'Start here'
                },
                {
                    image:'about-us-02-image-box-02.png',
                    title:'Customize Prefences',
                    info:'You can store online lessons via online cloud or download to your device and revise lessons on the way.',
                    linkText:'Get free guide'
                },
                {
                    image:'home-2-image-box-03.png',
                    title:'Customize Prefences',
                    info:'You can store online lessons via online cloud or download to your device and revise lessons on the way.',
                    linkText:'Start now'
                },
            ],
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/class.scss";
.smart-tutoring-section{
    background-color: rgb(255, 255, 255);
    border-bottom-right-radius: 500px;
}
.bottom-shadow{
    box-shadow: 0 40px 50px -30px rgb(97, 97, 97);
}
.youtube-logo{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>