<template>
    <a class="card-course col-6 d-flex align-items-center my-4"> 
        <img class="course-img" :src="getCourseImg()" alt="">
        <div class="ps-4">
            <h4 class="main-color-text fw-bolder"> {{getPrice(singleCourse.price)}} </h4>
            <h5> {{singleCourse.courseTitle }}</h5>
            <div>
                <span> <i class="bi bi-file-earmark-text"></i> {{ singleCourse.numLessons }} Lessons </span>
                <span> <i class="bi bi-person"></i> {{ singleCourse.numStudents }} Students </span>
            </div>
        </div>
    </a>
</template>

<script>
export default {
    props:{
        singleCourse:Object
    },
    methods:{
        getCourseImg(){
            return require('../assets/Images/'+ this.singleCourse.courseImg + '')
        },
        getPrice(price){
            if(price != 'Free'){
                return '$'+price+'.00'
            }
            return 'Free'
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
.course-img{
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
}
</style>