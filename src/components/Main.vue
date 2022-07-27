<template>
  <main>
    <!-- Sezione Corsi Online -->
    <OnlineCoursesSec/>

    <!-- Sezione Smart Tutoring -->
    <SmartTutoringSec/>

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
                <a href="#" class="main-btn-style" > Get Started now </a>
            </div>
        </div>
    </section>

    <!-- Sezione Risultati -->
    <ResultsSec/>

    <!-- Sezione Blogs -->
    <BestBlogs/>

    <section class="subscribe-section py-large">
        <div class="container position-relative px-5 py-2">
            <img class="position-absolute top-0 end-0" src="../assets/Images/maxcoach-shape-09.png" alt="">
            <img class="position-absolute top-50 end-0" src="../assets/Images/maxcoach-shape-02.png" alt="">
            <img src="" alt="">
            <div class="text-center subscribe-zone">
                <h3>Subscribe <span class="main-color-text fw-normal">Newsletters</span></h3>
                <p class="py-3">Enter your email address register to our newsletter subscription delivered on a regular basis!</p>
                <div class="input-group mb-3">
                    <input type="email" class="form-control" placeholder="Enter your email" aria-label="Recipient's username" aria-describedby="basic-addon2">
                    <div class="input-group-append">
                        <button class="main-btn-style"> Subscribe </button>
                    </div>
                </div>
            </div>
        </div>
    </section>
  </main>
</template>

<script>
import SmartTutoringSec from "../sections/SmartTutoringSec.vue"
import OnlineCoursesSec from "../sections/OnlineCoursesSec.vue"
import ResultsSec from "../sections/ResultsSec.vue"
import BestBlogs from "../sections/BestBlogs.vue"
export default {
    components:{
        SmartTutoringSec,
        ResultsSec,
        OnlineCoursesSec,
        BestBlogs,
    },
    data:function(){
        return{
           
            
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
main{
    background-color: $mainBgColor;
    .subscribe-section{
        background-color: white;
        .subscribe-zone{
            margin: 0 auto;
            width: 600px;
            input{
                border: none;
                background-color: $mainBgColor;
                padding-left: 20px;
            }
            button{
                height: 100%;
            }
        }
    }
}


</style>