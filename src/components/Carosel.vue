<template>
    <section >
        <div class="circle ">
            <i @click=" nextPg()" class="fas fa-sort-up"></i>
            <div class="numb my-2">{{visibitily+1}}/4</div>
            <i @click="prevPg()" class="fas fa-sort-down"></i>
        </div>
    <div class="row">
    <div  v-show="visibitily==index"  v-for="(info, index) in infoCarosel" :key="index" class="col-6 sez_1 text-center">
        <h5 class="my-5">{{info.title}}</h5>
        <div class="text">
           {{info.text}}
        </div>
        <img :src="info.img" alt="">
        <p>{{info.pg}}</p>
        <p>{{info.job}}</p>
    </div>


    <div class="col-6 img">
    </div>

    </div>
    </section>
</template>

<script>
export default {
name:"Carosel",
props:{
    infoCarosel:Array,
},
data(){
    return{
        visibitily: 0,
    }
},
methods:{

    show: function(){

    },
        nextPg: function(){

            this.visibitily++;
            if( this.visibitily >= this.infoCarosel.length){
                this.visibitily = 0;
            }
},
prevPg: function(){
            this.visibitily--;
            if(this.visibitily == -1){
                this.visibitily = this.infoCarosel.length-1;
            }

        },

    },
    
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