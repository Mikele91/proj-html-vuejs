<template>
    <header>
        <div class="container">
            <div class="header_top d-flex py-3">
                <img src="../assets/images/dark-logo.png" alt="">
                <div class="links_nav d-flex">
                <nav v-for ="(link, index) in infoNav" :key="index" class="d-flex "> 
                    <a href="#"> {{link}}  <i class="fas fa-chevron-down"></i> </a>
                </nav>
                </div>
                <div  class="icons d-flex "> 
                <div v-for ="(log, i) in infoMed" :key="i">
                    <a href="#"> <i :class= "`fab ${log}`"></i></a>                  
                </div>
                </div>




            </div>

                <div class="header_bottom">
                    <div class="row">
                        <div class="col-4">
                            <h4 class="pt-5">I'M WINGMAN</h4>
                            <h2>Peave On Earth A <br> Wonderful Wish  <br> But No Way</h2>
                            <p class="py-3">
                                Success isn't overnight. It's when everyday you get a little <br> better than the day before. it all adds up. 

                            </p>
                            <button> Get started for free <i class="fas fa-long-arrow-alt-right px-2"></i> </button>
                        </div>
                        <div class="col-8">
                            <div class="container_img">

                            <img src="../assets/images/home-movation-hero-image.png" alt="">
                            </div>
                        </div>
                    </div>
                </div>
        </div>
        <div class="shop d-flex flex-column">
            <div v-for="(icon, ind) in infoShop" :key="ind">
            <a href="#"><i :class="`far ${icon}`"></i> </a>
            </div>
            <!-- <a href="#"><i class="far fa-life-ring"></i></a>
            <a href="#"><i class="fas fa-book"></i></a>
            <a href="#"><i class="fas fa-shopping-cart"></i></a> -->
        </div>
    </header>
</template>

<script>
export default {
    name:"Header",
    props:{
        infoNav:Array,
        infoMed:Array,
        infoShop:Array,
    }
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
header{
    position: relative;
    background-color: $amoru;
    background-image: $backMain;
    .header_top{
        justify-content: space-between;
        align-items: center;
        .links_nav a i{
            font-size: 8px;
        }
        img{
            width: 12.5rem;
        };
    }
    .header_bottom{
        .col-4{
            h4{
                font-size: 0.7rem;
            }
        }
        .col-8{
            .container_img {
                margin-left: 50px ;
                width: 400px;
                background-image: url('../assets/images/home-movation-shape-face.png');
                background-repeat: no-repeat;
                background-size: 350px 300px;
                background-position: right;
                background-position-y: bottom;
            
            img{
                height: 400px
            }
        }
        };
    }
    .shop{
        align-items: center;
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-70% );
        background-color: white;
        a{
          
            color: black;
            i{
                padding: 12px 0;
            }
        } 
    }
}
</style>