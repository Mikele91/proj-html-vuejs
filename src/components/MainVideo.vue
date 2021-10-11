<template>
    <section>
        <div class="row ">
        <p> <span>ABOUT ME</span> </p>
            <div class="col-3">
                <h2>How To Be an Alpha Male: THe 15 Habits of True Alphas</h2>
            </div>
            <div class="col-9  ">
                <div class="description">
                    <h4>Want to learn how to be <span>alpha male?</span> How to be more mascukune?</h4>
                    <h4>How to be the man you've always wanted to be ?</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem, natus? Mollitia vero itaque asperiores maxime consectetur repellendus excepturi, provident nisi, quis distinctio assumenda accusamus voluptatem ducimus cumque odio molestiae! Reiciendis.</p>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col-6 my-5">
                <div>
                <img id="motivator" src="../assets/images/home-movation-video-poster-670x450.jpg" alt="#">
                <a href="https://www.youtube.com/watch?v=2MvsvdjlhIs&ab_channel=DavidPrastyawan" target="_blank">
                    <img class="youtube" src="../assets/images/icon-youtube-play.png" alt="#">
                    </a>

                </div>
            </div>
             <div class="col-6 ">
                <div class="container_motivation">
                    <p >
                        "Every morning you have twe choices: continue to sleep with your dreams, or wake up and chase them."
                    </p>
                    <div>
                        <img src="../assets/images/home-movation-shape-01.png" alt="">
                    </div>
                    <h5 class="py-3"> <strong>Tony Stark</strong> </h5>
                    <p class="about">Wingman</p>

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name:"Main.Video",
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
section{

    span{
        color: $jungle;
    }
    .description{
        margin-left: 200px;
    }
    .description h4{
        font-size:15px;
        font-weight: 700;
    }
    .col-6 div{
        position: relative;
    }
        .youtube{
            position: absolute;
            top:50%;
            left: 50%;
            transform: translate(-50%, -50%);
    }
    #motivator{
        width: 100%;
    }
    .container_motivation {
        padding:6rem 7rem;
        font-weight:  700;
        font-size: 2rem;
        p:last-child{
            font-size: 1rem
            }
    }
}
</style>