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
    <section class="best-blog-section py-5">
        <div class="container">
            <div class="d-flex gap-3">   
                <div class="col-4">
                    <span class="d-block"> ENJOYABLE INSIGHTS </span>
                    <h2>Most Viewed Best Blogs</h2>
                    <ul>
                        <li v-for="(blog) in bestBlogs" :key="blog.id" class="my-4">
                            <a href="#">-->  {{ blog.title }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-4 bg-danger">
                    Card
                </div>
                <div class="col-4 bg-danger">
                    Card
                </div>
            </div>        
        </div>
    </section>
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
export default {
    components:{
        SmartTutoringSec,
        ResultsSec,
        OnlineCoursesSec,
    },
    data:function(){
        return{
           
            bestBlogs:[
                {
                    id:10,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:11,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:15,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:20,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:18,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
            ]

        }
    }
}
</script>

<style lang="scss">
main{
    background-color: #f6f3f5;
}
.best-blog-section{
    background-color: lightgrey;
}
</style>