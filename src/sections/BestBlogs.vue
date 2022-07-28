<template>
   <section class="best-blog-section py-5">
        <div class="container py-5">
            <div class="d-flex  align-items-center col-12">   
                <div class="col-4">
                    <span class="d-block subtitle-text"> ENJOYABLE INSIGHTS </span>
                    <h2 class="py-3">Most Viewed Best Blogs</h2>
                    <ul>
                        <li v-for="blog in bestBlogs" :key="blog.id" class="my-4">
                            <a href="#" class="fw-bolder"> <i class="bi bi-arrow-right"></i>  {{ blog.title }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-4 ps-5" v-for="prevblog in previewBlogs" :key="prevblog.id">
                    <CardBlog
                    :blog="prevblog"
                    />
                </div>
            </div>        
        </div>
    </section>
</template>

<script>
import CardBlog from "./cards/CardBlog.vue"
export default {
    components:{
        CardBlog,
    },
    data:function(){
        return{
            previewBlogs:[
        {
            id:80,
            image:"artist-blog-03-480x352.jpeg",
            type:'Artist',
            title:'Become a Better Blogger:Content Planning',
            lastUpdate:'26/07/2022',
            view:688,
        },
        {
            id:90,
            image:"artist-blog-01-480x352.jpg",
            type:'Artist',
            title:'Pocket-Sized Notebooks Hold Miniature Paintings',
            lastUpdate:'26/07/2022',
            view:688,
        }

    ],
    bestBlogs:[
                {
                    id:10,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:11,
                    type:'Artist',
                    title:'Promoting Your Online Business On Pinterest',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:15,
                    type:'Artist',
                    title:'Designing an Online Course from Expert\'s Perspective',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
                {
                    id:20,
                    type:'Artist',
                    title:'Become a Better Blogger:Content Planning',
                    lastUpdate:'26/07/2022',
                    view:688,
                },
            ]
        }
    }
    
}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/class.scss";

</style>