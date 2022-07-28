<template>
  <footer class="py-5">
    <div class="container">
        <div class="d-flex pb-5">
            <div class="col-6">    
                <h5>Address</h5>
                <ul>
                    <li> {{this.contactInfo.address}} </li>
                    <li class="my-2"> {{this.contactInfo.phone}}</li>
                    <li> {{this.contactInfo.email}}</li>
                </ul>
                <div class="my-2 social second-color-text">
                    <a href="#"><i class="bi bi-facebook"></i></a>
                    <a href="#"><i class="bi bi-twitter"></i></a>
                    <a href="#"><i class="bi bi-instagram"></i></a>
                    <a href="#"><i class="bi bi-linkedin"></i></a>
                </div>
            </div>
            <div class="col-6 d-flex">
                <div>
                    <h6 class="pb-3">Information </h6> 
                    <div class="d-flex align-items-center">
                        <ul class="">                          
                        <li  class="secondary-color-text">
                           <a href="#" class="footer-link">Start Here</a>
                        </li>
                        <li class="secondary-color-text my-2">
                            <a href="#" class="footer-link">Blog</a> 
                        </li>
                        <li class="secondary-color-text">
                            <a href="#" class="footer-link">About Us</a> 
                        </li>                                    
                    </ul>
                    <ul class="ms-5">                          
                        <li  class="secondary-color-text">
                           <a href="#" class="footer-link">Success Story</a>
                        </li>
                        <li class="secondary-color-text my-2">
                            <a href="#" class="footer-link">Course</a> 
                        </li>
                        <li class="secondary-color-text">
                            <a href="#" class="footer-link">Contact us</a> 
                        </li>                                    
                    </ul>
                    </div>                    
                </div>
                <div class="ms-5">
                    <h6 class="pb-3">Information </h6>
                    <ul>
                        <li class="my-2" v-for="(link,index) in informations" :key="index">
                            <a href="#" class="footer-link">{{link.name}}</a>
                        </li>
                    </ul>
                </div>
               
            </div>
        </div> 
        <div class="copyright text-center">
            <span class="small-text-color">@ 2020 Maxcoach,All Rights Reserved</span>   
        </div> 
    </div>
    <a href="#start-page" class="anchor"><i class="fs-3 bi bi-arrow-up"></i>
</a> 
  </footer>
</template>

<script>
export default {
    data:function(){
        return{
            contactInfo:{
                address:'382 NE 191st St # 87394 Miami,FL 33179-3899',
                phone:'305 547-9909',
                email:'support@maxcoach.com'
            },
            exploreLinks:[
                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'Start here'
                },
                                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'Blog'
                },
                                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'About us'
                },
                                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'Success story'
                },
                                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'Courses'
                },
                                {
                    urlLink:'pdapldpsladp.org',
                    linkText:'Contact us'
                },

            ],
            informations:[
                {
                    urlLink:'dasdasdas',
                    name:'Membership'
                },
                {
                    urlLink:'dasdasdas',
                    name:'Purchase guide'
                },
                {
                    urlLink:'dasdasdas',
                    name:'Privacy policy'
                },
                {
                    urlLink:'dasdasdas',
                    name:'Terms of services'
                },
            ]

        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/class.scss";
    footer{
        background-color:$mainBgColor;
        position:relative;
        .anchor{
            padding: 30px;
            position: absolute;
            bottom: 50px;
            right: 50px;
            color: white;
            border-radius: 50%;
            line-height: 0;
            background-color: $mainColor;
        }
        .social i{
            margin:0 10px;
            color: $smallTextColor;
        }
        .footer-link{
            font-size: 14px;
        }
    }
</style>