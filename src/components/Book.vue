<template>
  <section>
      <div class="main_top ">
        <div class="row">
          <div class="col-5">
            <p>
              BOOK STORE ONLINE
            </p>
            <h2> Be Alpha With <span>Wingmans's Book</span> </h2>
              <section class="list my-5">

              <div> <i class="fas fa-check me-2"></i>Help you understand youself better</div>
              <div> <i class="fas fa-check me-2"></i>Revealing mature tips</div>
              <div> <i class="fas fa-check me-2"></i>Give the right advice</div>
              <div> <i class="fas fa-check me-2"></i>Fascinating examples of alpha man</div>
            
              </section>
            <button> Get Free Ebook</button>
          </div>
          <div class="col-7">
            <div class="row">
              <div class="col-6 text-center">
                <img src="../assets/images/product-book-11-400x400.jpg" alt="">
                  <p>How to be Successful</p>
                 <div class="price"> $20.00</div>
              </div>
              <div class="col-6 text-center ">
                <img src="../assets/images/product-book-10-400x400.jpg" alt="">
                        <p>Create  Success</p>
                        <div class="price"> $30.00</div>
              </div>

            </div>
          </div>
        </div>
      </div>
      <div class="main_icon my-5 d-flex">
        <img src="../assets/images/client-logo-01-primary.png" alt="">
        <img src="../assets/images/client-logo-02-primary.png" alt="">
        <img src="../assets/images/client-logo-03-primary.png" alt="">
        <img src="../assets/images/client-logo-04-primary.png" alt="">
        <img src="../assets/images/client-logo-05-primary.png" alt="">
        <img src="../assets/images/client-logo-06-primary.png" alt="">
        <img src="../assets/images/client-logo-07-primary.png" alt="">






      </div>
  </section>
</template>

<script>
export default {
nome:"Book",
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
.col-5{
  p{
    color:$grey
  
  }

h2{
  font-weight: 500;
  font-size: 3rem;
  span{
    color:$jungle;
  }
}
.list{
  i{
    margin: 0.5rem 0;
    font-size: 20px;
    color:$jungle
  }
}
}
.col-6{
    transition: transform .2s;

    &:hover{
      transform: scale(1.1)
    }
  img{
    width: 300px;
  }
  p{
    color:$grey;
    font-weight: 700;

  }
  .price{
          color:$jungle;
          font-weight: 700;
          font-size: 1.5rem;
          margin: 1rem 0;
  }
}
  .main_icon{
    justify-content: space-between;
    align-items: center;
    img{
      opacity: 0.2;
      &:hover{
      opacity: 1;
      }
    }
  }
</style>