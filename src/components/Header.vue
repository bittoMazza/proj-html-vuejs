<template>
  <header >
    <div class="header-container" id="start-page">
        <div class="container-nav d-flex justify-content-between container align-items-center py-3">
        <img class="logo-navbar" src="../assets/Images/dark-logo.png" alt="logo-dark">
        <nav class="d-flex align-items-center">    
            <ul class="second-text-color">
                <li v-for="(link,index) in navLinks" :key="index" class="px-3">
                    <a href="#">{{link}}<i class="ms-1 bi bi-chevron-down"></i></a>
                </li>
            </ul>
            <a href="#" class="fs-5"><i class="me-3 bi bi-person-circle"></i></a>
            <div class="input-search ms-2">
                <input type="text" class="" placeholder="Search...">
                <button class="search-button"><i class="bi bi-search main-color-text"></i></button>
            </div>     
        </nav>
        </div>
    </div>  
    <IntroductionSec/>
  </header>
</template>

<script>
import IntroductionSec from '../sections/IntroductionSec.vue'
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
@import "../styles/class.scss";
.header-container{

        box-shadow: 0 5px 10px -5px rgb(222, 221, 221);
        .input-search{
            background-color: $mainBgColor;
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

 .search-button{
                border:none;
                height: 100%;
                background-color: $mainBgColor;
            }
</style>