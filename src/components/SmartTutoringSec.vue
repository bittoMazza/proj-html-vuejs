<template>
  <section class="py-5 smart-tutoring-section">
        <div class="container px-5">
            <div class="text-center">
                <span> GREAT WORDS ABOUT MAXCOACH </span>
                <h3> Access Smart Tutoring Program For Benefits </h3>
            </div>
            <div class="d-flex py-5">
                <CardSmartTutoring v-for="(benefit,index) in tutoringBenefits" :key="index"
                :cardBenefit="benefit"
                />
            </div>
            <div class="py-5 d-flex align-items-center"> 
                <div class="col-8 ps-3">
                    <img class="" src="../assets/Images/home-2-popup-video-poster.jpg" alt="">                
                </div>
                <div class="col-4 pe-3">
                    <span>GET STARTED <span>EFFORTLESSLY</span></span>
                    <h2>Enjoy Our Companionship</h2>
                    <p>Learning is a life-long journey that in fact we nerver finda the terminate stop. Stop searching,enjoy the process.</p>
                    <a href="#">Download the guidebook --></a>
                </div>   
            </div>          
        </div>
    </section>
</template>

<script>
import CardSmartTutoring from './CardSmartTutoring.vue'
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

</style>