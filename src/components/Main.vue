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

    <section class="subscribe-section py-5">
        <div class="container">
            <div class="text-center">
                <h3>Subscribe Newsletters</h3>
                <p>Enter your email address register to our newsletter subscription delivered on a regular basis!</p>
                <div>
                    <input type="email" placeholder="Enter your email">
                    <button> Subscribe </button>
                </div>
            </div>
        </div>
    </section>
  </main>
</template>

<script>
import SmartTutoringSec from "./SmartTutoringSec.vue"
import OnlineCoursesSec from "./OnlineCoursesSec.vue"
import ResultsSec from "./ResultsSec.vue"
import BestBlogs from "./BestBlogs.vue"
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
main{
    background-color: #f6f3f5;
    .subscribe-section{
        background-color: white;
    }
}


</style>