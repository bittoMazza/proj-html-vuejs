<template>
  <main>
    <section class="py-5 online-courses-section">
        <div class="container px-5">
            <div class="text-center">
                <span> STIMULATED TO LEARN? </span>
                <h3> Featured Online Courses </h3>
            </div>
            <div class="d-flex flex-wrap">
                 <CardCourse  v-for="course in OnlineCourses" :key="course.id"
                 :singleCourse ="course"
                 />
            </div>   
            <div class="text-center pt-5">
                <a href="#" class="btn-style"> View all courses </a>    
            </div> 
        </div>     
    </section>
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
    <section class="py-5 top-learners-section">
        <div class="container-fluid">
            <div>
                <div class="text-center">
                    <span> GREAT WORDS ABOUT MAXCOACH </span>
                    <h3> Access Smart Tutoring Program For Benefits </h3>
                </div>
                
                <div class="d-flex"> 
                    <div class="col-4">
                        card
                    </div>
                    <div class="col-4">
                        card
                    </div>
                    <div class="col-4">
                        card
                    </div>
                </div>
            </div>
            <div class="text-center py-5">
                <h5>Start today for getting Online Certification </h5>
                <h3 class="pb-5">You can be your own guiding star with out help</h3>
                <a href="" class="btn-style"> Get Started now </a>
            </div>
        </div>
    </section>
    <section class="results-section">
        <div class="container">
            <div class="d-flex">
                <CardResults v-for="(resultInfo,index) in results" :key="index"
                :resultData ="resultInfo"
                />
            </div>
        </div>
    </section>
  </main>
</template>

<script>
import CardSmartTutoring from "./CardSmartTutoring.vue"
import CardCourse from "./CardCourse.vue"
import CardResults from "./CardResults.vue"
export default {
    components:{
        CardCourse,
        CardSmartTutoring,
        CardResults,
    },
    data:function(){
        return{
            OnlineCourses:[
                {
                    id:16,
                    courseImg:'course-02-480x298.jpg',
                    price:'40',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                },
                {
                    id:25,
                    courseImg:'stock-full-hd-03-480x298.jpg',
                    price:'Free',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                },
                {
                    id:33,
                    courseImg:'stock-full-hd-04-480x298.jpg',
                    price:'19',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                },
                {
                    id:1,
                    courseImg:'stock-full-hd-06-480x298.jpg',
                    price:'26',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                },
                {
                    id:4,
                    courseImg:'course-featured-image-01-480x298.jpg',
                    price:'39',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                },
                {
                    id:11,
                    courseImg:'stock-full-hd-05-480x298.jpg',
                    price:'59',
                    courseTitle:'Learning to Write as a Professional Author',
                    numLessons:20,
                    numStudents:50,

                }
            ],
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
            results:[
                {
                    title:'Succesfully trained',
                    num:1790,
                    numInfo:'ENROLLED LEARNERS'
                },
                {
                    title:'Proudly Received',
                    num:19,
                    numInfo:'ENROLLED LEARNERS'
                },
                {
                    title:'Fimly Established',
                    num:24,
                    numInfo:'ENROLLED LEARNERS'
                },
                {
                    title:'Succesfully trained',
                    num:1090,
                    numInfo:'ENROLLED LEARNERS'
                },
            ]

        }
    }
}
</script>

<style lang="scss">
.online-courses-section{
    background-color: rgb(218, 240, 232);
}
.btn-style{
    text-decoration: none;
    border-radius: 5px;
    padding: 10px 20px;
    background-color: blanchedalmond;
}
.smart-tutoring-section{
    background-color: rgb(255, 255, 255);
    border-bottom-right-radius: 500px;
}
.top-learners-section{
    background-color: rgb(222, 253, 243);
}
</style>