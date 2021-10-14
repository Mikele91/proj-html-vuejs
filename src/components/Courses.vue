<template>
    <section>
            <header class="text-center">
                <h5>BEGIN YOUR JOURNEY AT MAXCOACH</h5>
                <h2 class="mb-5"> Lastes <span>Online Courses</span></h2>
            </header>
            <main>


                <!-- sezione card  -->
                <div class="row">
                    <!-- prima riga  -->
                    <div v-for="(info, index) in infoCourses" :key="index" class="col-4 my-5">
                        <img :src="info.imge" alt="">
                        <div class="text container">
                            <div class="price"> {{info.price}}</div>
                            <p>{{info.text}}</p>
                            <span v-for="(icon, i) in info.icons" :key="i" class="icons">
                                <i :class="icon"></i> <span class="m-3"> {{icon.text}}</span>
                            </span>  
                        </div>
                    </div>
                </div>


                    <!-- SEZIONE LINK  -->
                <div class="row">
                    <div class="col-12 text-center">
                        <button class="my-5">
                            View all courses <i class="fas fa-long-arrow-alt-right ps-2"></i>
                        </button>
                    </div>
                </div>
            </main>
    </section>
</template>

<script>
export default {
name:"Courses",
props:{
    infoCourses:Array
}
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
section{
header{
    h5{
        color:$grey;
        font-size: 1rem;
    }
    h2{
        font-size: 3rem;
        span{
            color:$jungle
        }
    }
}
main{
    .col-4{
        transition: .5s;
        &:hover{
            box-shadow: 0 10px rgba(128, 128, 128, 0.062) ;
            transform: scale(1.1)
        }
        p{
            color: $marino;
            font-weight: 700;
        }
        .icons{
            color:$grey
        }

    }
    img{
        margin:0, 1rem;
        width: 25rem;
        border-radius: .3125rem;
    }
    .price{
        color:$jungle;
        font-weight: 700;
        font-size: 1.5rem;
        margin: 1rem 0;
    }
}
}
</style>