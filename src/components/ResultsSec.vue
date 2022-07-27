<template>
  <section class="results-section">
        <div class="container">
            <div class="d-flex">
                <CardResults v-for="(resultInfo,index) in results" :key="index"
                :resultData ="resultInfo"
                />
            </div>
        </div>
    </section>
</template>

<script>
import CardResults from "./CardResults.vue"
export default {
    components:{
        CardResults,
    },
    data:function()
    {
        return{
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
            ],
        }
    }
}
</script>

<style>

</style>