<template>
    <div class="card-course col-6 d-flex my-4"> 
        <img class="course-img" :src="getCourseImg()" alt="">
        <div>
            <h4> {{singleCourse.price}} </h4>
            <h5> {{singleCourse.courseTitle }}</h5>
            <div>
                <span> {{ singleCourse.numLessons }} Lessons </span>
                <span> {{ singleCourse.numStudents }} Students </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        singleCourse:Object
    },
    methods:{
        getCourseImg(){
            return require('../assets/Images/'+ this.singleCourse.courseImg + '')
        }
    }
}
</script>

<style>
.course-img{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    object-fit: cover;
}
</style>