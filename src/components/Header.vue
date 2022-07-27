<template>
  <header >
    <div class="header-container" id="start-page">
        <div class="container-nav d-flex justify-content-between container align-items-center py-3">
        <img class="logo-navbar" src="../assets/Images/dark-logo.png" alt="logo-dark">
        <nav class="d-flex align-items-center">    
            <ul>
                <li v-for="(link,index) in navLinks" :key="index" class="px-3">
                    <a href="#">{{link}}</a>
                    <i class="ms-2 bi bi-chevron-down"></i>
                </li>
            </ul>
            <a href="#"><i class="me-3 bi bi-person-circle"></i></a>
            <div class="input-search">
                <input type="text" placeholder="Search...">
                <i class="bi bi-search"></i>
            </div>     
        </nav>
        </div>
    </div>  
    <IntroductionSec/>
  </header>
</template>

<script>
import IntroductionSec from './IntroductionSec.vue'
export default {
    components:{
        IntroductionSec,
    },
    data:function(){
        return{
            navLinks:['Home','Pages','Courses','Features','Blog','Shop']
        }
    },
    
}
</script>

<style lang="scss">
@import "../styles/variables.scss";

.header-container{

        box-shadow: 0 5px 5px -5px #333;
        .input-search{
            background-color: blue;
            padding: 10px 10px;
            input{
                border: none;
                background-color: transparent;
            }
        }
        .container-nav{
            nav ul{
            margin: 0;
            }
            .logo-navbar{
                height: 25px;
            }   
            nav ul li{
            list-style: none;
            display: inline-block;
        }
        }
    }


</style>