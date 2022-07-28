<template>
  <section class="py-5 top-learners-section">
        <div class="container-fluid">
            <div>
                <div class="text-center">
                    <span class="subtitle-text"> GREAT WORDS ABOUT MAXCOACH </span>
                    <h3 class="fw-bold bold-text-color"> Our <span class="h3 main-color-text fw-normal">top learner's </span>verbatim </h3>
                </div>
                
                <div class="d-flex py-4"> 
                    <CardLearner v-for="(card,index) in learners" :key="index"
                    :learner="card"
                    />
                </div>
            </div>
            <div class="text-center py-5">
                <div class="online-certification-box px-5 position-relative">  
                    <i class="bi bi-circle position-absolute bottom-50 start-0 circle-bg-image"></i>  
                    <img class="position-absolute top-50 start-0" src="../assets/Images/maxcoach-shape-01.png" alt=""> 
                    <img class="position-absolute top-50 end-0" src="../assets/Images/maxcoach-shape-02.png" alt="">
                    <h5>Start today for getting <span class="h5 main-color-text fw-normal">Online Certification </span></h5>
                    <h3 class="pb-5">You can be your own guiding star with out help</h3>
                    <a href="#" class="main-btn-style" > Get Started now </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import CardLearner from './cards/CardLearner.vue'
export default {
    data: function () {
        return {
            learners: [
                {
                    title: "High level of efficency and scintific teaching methods",
                    textContent: "I am free to learn at my own pace,follow my own schedule and choose the subject. I want to learn from the syllabus. Great study portal for people like me",
                    image: require('../assets/Images/learners/testimonial-avata-02.jpg'),
                    name: "MINA HOLLACE",
                    position: "Freelancer"
                },
                {
                    title: "High level of efficency and scintific teaching methods",
                    textContent: "I am free to learn at my own pace,follow my own schedule and choose the subject. I want to learn from the syllabus. Great study portal for people like me",
                    image: require("../assets/Images/learners/testimonial-avata-01.jpg"),
                    name: "CICCIO PASTICCIO",
                    position: "Freelancer"
                },
                {
                    title: "High level of efficency and scintific teaching methods",
                    textContent: "I am free to learn at my own pace,follow my own schedule and choose the subject. I want to learn from the syllabus. Great study portal for people like me",
                    image: require("../assets/Images/learners/testimonial-avata-03.jpg"),
                    name: "FLORENZ THEMES",
                    position: "Freelancer"
                }
            ]
        };
    },
    components: { CardLearner }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/class.scss";
.online-certification-box{
    margin: 0 300px;
}

</style>