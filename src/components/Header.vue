<template>
    <header>
           <div class="container">
               <div class="header_top d-flex py-3">
                <img src="../assets/images/dark-logo.png" alt="">
                <nav class="d-flex "> 
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>
                    <a href="#"> Home  <i class="fas fa-chevron-down"></i> </a>


                

                </nav>
                <div class="icons d-flex">
                    <a href="#"> <i class="fab fa-twitter"></i></a>
                    <a href="#"> <i class="fab fa-facebook-f"></i></a>
                     <a href="#"> <i class="fab fa-instagram"></i></a>
                     <a href="#"> <i class="fab fa-linkedin"></i></a>
                    
                    
                </div>




                <div class="header_bottom"></div>
               </div>
           </div>
    </header>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
header{
     background-image: $backMain;
     .header_top{
         justify-content: space-between;
         align-items: center;
         img{
             width: 12.5rem;
         }
     };
}
</style>