<template>
  <main>
    <section class="py-5 online-courses-section">
        <div class="container">
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
  </main>
</template>

<script>
import CardCourse from "./CardCourse.vue"
export default {
    components:{
        CardCourse,
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
            ]
        }
    }
}
</script>

<style lang="scss">
.online-courses-section{
    background-color: aquamarine;
}
.btn-style{
    text-decoration: none;
    border-radius: 5px;
    padding: 10px 20px;
    background-color: blanchedalmond;
}
</style>