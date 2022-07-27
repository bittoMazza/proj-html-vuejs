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
import CardResults from "./cards/CardResults.vue"
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
                    numInfo:'COUNTRYWIDE AWARDS'
                },
                {
                    title:'Fimly Established',
                    num:24,
                    numInfo:'LOCAL BRANCHES'
                },
                {
                    title:'Succesfully trained',
                    num:1090,
                    numInfo:'BLOG POSTS'
                },
            ],
        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
.results-section{
    background-color: white;
}
</style>