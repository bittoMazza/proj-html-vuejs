<template>
  <footer class="py-5">
    <div class="container">
        <div class="d-flex">
            <div class="col-6">    
                <h5>Address</h5>
                <ul>
                    <li> {{this.contactInfo.address}} </li>
                    <li class="my-2"> {{this.contactInfo.phone}}</li>
                    <li> {{this.contactInfo.email}}</li>
                </ul>
                <div class="my-2 social">
                    <a href="#"><i class="bi bi-facebook"></i></a>
                    <a href="#"><i class="bi bi-twitter"></i></a>
                    <a href="#"><i class="bi bi-instagram"></i></a>
                    <a href="#"><i class="bi bi-linkedin"></i></a>
                </div>
            </div>
            <div class="col-6 d-flex">
                <ul class="px-2">    
                    <li class="h6">Explore</li>
                    <li>dad</li>
                    <li>dad</li>
                </ul>
                <ul class="px-2">
                     <h6>Information</h6>
                    <li>p</li>
                </ul>
                <ul class="px-2">
                     <h6>Information</h6>
                    <li>
                        
                    </li>
                </ul>
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
                address:'Indirizzo e via',
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

            ]

        }
    }
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
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
    }
</style>