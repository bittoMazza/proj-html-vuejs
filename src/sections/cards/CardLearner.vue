<template>
  <div class="col card-container py-5 px-5 mx-3">
    <h5>{{learner.title}}</h5>
    <p class="py-2 fw-bold second-text-color">{{learner.textContent}}</p>
    <div class="d-flex align-items-center">
        <img class="avatar" :src="learner.image" alt="">
        <div class="ms-3">
            <h6>{{learner.name}}</h6>
            <span class="small-text-color">{{learner.position}}</span>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    props:{
        learner:Object
    }
}
</script>

<style>
@import "../../styles/variables.scss";
.card-container{
    background-color: white;
    border-radius: 5px;
}
.avatar{
    width: 60px;
    border-radius: 50%;
}
</style>