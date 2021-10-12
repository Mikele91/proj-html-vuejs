<template>
    <section >
        <div class="circle ">
            <i class="fas fa-sort-up"></i>
            <div class="numb my-2">1/4</div>
            <i class="fas fa-sort-down"></i>
        </div>
    <div class="row">
    <div class="col-6 sez_1 text-center">
        <h5 class="my-5">REAL STORIES</h5>
        <div class="text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa magnam laborum vitae nesciunt id labore dicta sed soluta cumque iusto laboriosam hic quas, sit minus voluptatum debitis a necessitatibus voluptatibus!
        </div>
        <img src="../assets/images/testimonial-avata-02.jpg" alt="">
        <p>Mina Hollace</p>
        <p>/Freelabcer</p>
    </div>

    <div class="col-6 img">
    </div>

    </div>
    </section>
</template>

<script>
export default {
name:"Carosel"
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';

section{
    position: relative;
    .circle{
        width: 6rem;
        height: 6rem;
        border-radius: 50%;
        background-color: white;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        i{
            cursor: pointer;
        }

    }
}
.sez_1{
    background-color: $amoru;
    background-image: $backMain;
    h5{
        color:$jungle
    }
    .text{
        width: 50%;
        margin:auto
    }
    img{
        margin: 3rem 0;
        width: 100px;
        border-radius: 50%;
    }
    p:last-child{
        color:$grey;
        font-size: 0.7rem;
    }
}
.img{
        height: 500px;
        background-image: url('../assets/images/home-movation-testimonial-image.jpg') ;
        background-size: cover;
        background-position:center;
    
}

</style>