<template>
    <section>
            <header class="text-center">
                <h5>BEGIN YOUR JOURNEY AT MAXCOACH</h5>
                <h2 class="mb-5"> Lastes <span>Online Courses</span></h2>
            </header>
            <main>
                <div class="row">
                    <div class="col-4 ">
                        <img src="../assets/images/motivation-course-06-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">
                            <i class="fas fa-book  my-5"></i> <span class="mx-2"> 3 Lessons</span>
                            <i class="far fa-user ms-5 "></i> <span class="mx-2"> 50 Students</span>
                        </div>
                            
                        </div>
                    </div>
                      <div class="col-4">
                          <div class="container">
                              
                          </div>
                        <img src="../assets/images/motivation-course-05-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">

                        </div>
                            
                        </div>
                    </div>
                      <div class="col-4 ">
                        <img src="../assets/images/motivation-course-04-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">

                        </div>
                            
                        </div>
                    </div>
                    

                      <div class="col-4 ">
                        <img src="../assets/images/motivation-course-03-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">

                        </div>
                            
                        </div>
                    </div>
                      <div class="col-4">
                        <img src="../assets/images/motivation-course-02-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">

                        </div>
                            
                        </div>
                    </div>
                      <div class="col-4 ">
                        <img src="../assets/images/motivation-course-01-480x298.jpg" alt="">
                        <div class="text container">
                        <div class="price"> $30.00</div>
                        <p>How to be Successful: create a Growt Mindset For Success</p>
                        <div class="icons">

                        </div>
                            
                        </div>
                    </div>
                </div>
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
name:"Courses"
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