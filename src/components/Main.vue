<template>
<main>
    <!-- sezione con container del main  -->
    <div class="main_top container my-5">
    <section class="price">
        <div class="row">
            <div class="col-3 text-center">
                <div class="price_number ">
                    1.926
                </div>
                <div class="text_price">
                    FINISHED SESSION
                </div>

            </div>
              <div class="col-3 text-center">
                <div class="price_number ">
                    100%
                </div>
                <div class="text_price">
                    SATISFACTION RATE
                </div>

            </div>
              <div class="col-3 text-center">
                <div class="price_number ">
                   3092+
                </div>
                <div class="text_price">
                   ELLORED LEARNERS
                </div>
                

            </div>
              <div class="col-3 text-center">
                <div class="price_number ">
                    200
                </div>
                <div class="text_price">
                    ONLINE INSTRUCTORS
                </div>

            </div>
        </div>

    </section>
    <MainVideo/>
    <Courses :infoCourses="infoCourses"/>
    <Book/>

    </div>

    <div class="main_full">
        <Carosel :infoCarosel="infoCarosel"/>
    </div>
    <div class="main_bottom container my-5">
        <Blog/>

    </div>
</main>
        
</template>

<script>
import MainVideo from './MainVideo.vue'
import Courses from './Courses.vue'
import Book from './Book.vue'
import Carosel from './Carosel.vue'
import Blog from './Blog.vue'




export default {
    name:"Main",
    components:{
        MainVideo,
        Courses,
        Book,
        Carosel,
        Blog,
    },
    props:{
        infoCourses:Array,
        infoCarosel:Array,
    }
    

}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
main{
    .col-3{
        border-right:2px dashed $jungle;
        &:first-child{
            border-left: 2px dashed $jungle;
        }
    };
    .price{
        margin-bottom: 150px;
    }
    .price_number{
                font-size: 2rem;
                font-weight: 700;
                color:$jungle
            }
    // .main_bottom{
    //     height: 50px;
    //     background-color: red;
    // }
}

</style>