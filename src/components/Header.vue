<template>
  <header >
    <div class="d-flex justify-content-between container align-items-center py-3">
        <img class="logo-navbar" src="../assets/Images/dark-logo.png" alt="logo-dark">
        <nav class="d-flex align-items-center">    
            <ul>
                <li v-for="(link,index) in navLinks" :key="index" class="px-3">
                    {{link}}
                </li>
            </ul>
        <span class="px-2">User</span>
        <div>
            <input type="text" placeholder="Search...">
            <span>Icona</span>
        </div>S      
    </nav>
    </div>
    <section class="py-4">
        <div class="container">
            <div class="d-flex align-items-center my-4">
                <div class="col-5">
                    <h2>Distant learning for further expansion</h2>
                    <p>Learning is a life-long journey that in fact we nerver finda the terminate stop. Stop searching,enjoy the process.</p>
                    <button class="my-2"> Download free guide </button>
                    <span class="d-block">Have questions? <a href="#">Get Free Sample --></a></span>
                </div>
                <div class="col-7">
                    <img src="../assets/Images/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" class="rounded-circle w-100" alt="">
                </div>
            </div>
            <div class="clients-logo d-flex justify-content-between">
                <div v-for="(client,index) in 6" :key="index">
                    <img :src="getClientImg(index)" alt="">    
                </div>
            </div>
        </div>
    </section>
  </header>
</template>

<script>
export default {
    data:function(){
        return{
            navLinks:['Home','Pages','Courses','Features','Blog','Shop']
        }
    },
    methods:{
        getClientImg(ind){
            return require('../assets/Images/client_logo/client-logo-0'+(ind+1)+'.png')
        }
    }
}
</script>

<style lang="scss">

nav ul li{
    list-style: none;
    display: inline-block;
}
nav ul{
    margin: 0;
}
.logo-navbar{
    height: 25px;
}

</style>