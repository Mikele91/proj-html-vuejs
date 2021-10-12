<template>
  <section>
      <h4>Blog Update</h4>
      <h2>Interesting <span>articles updated</span>daily</h2>
      <div class="row">
          <div class="col-3 my-5">
              <img src="../assets/images/motivation-blog-04-480x325.jpg" alt="">
              <div class="date my-4"> <i class="far fa-calendar"></i> May 13, 2020</div>
              <h3> How to stay true to Your Personal Brand</h3>
              <p> When it comes tho your businesss or career, you want ...</p>
          </div>
           <div class="col-3 my-5">
              <img src="../assets/images/motivation-blog-03-480x325.jpg" alt="">
              <div class="date my-4"> <i class="far fa-calendar"></i> May 13, 2020</div>
              <h3> How to stay true to Your Personal Brand</h3>
              <p> When it comes tho your businesss or career, you want ...</p>
          </div>
           <div class="col-3 my-5">
              <img src="../assets/images/motivation-blog-02-480x325.jpg" alt="">
              <div class="date my-4"> <i class="far fa-calendar"></i> May 13, 2020</div>
              <h3> How to stay true to Your Personal Brand</h3>
              <p> When it comes tho your businesss or career, you want ...</p>
          </div>
           <div class="col-3 my-5">
              <img src="../assets/images/motivation-blog-01-480x325.jpg" alt="">
              <div class="date my-4"> <i class="far fa-calendar"></i> May 13, 2020</div>
              <h3> How to stay true to Your Personal Brand</h3>
              <p> When it comes tho your businesss or career, you want ...</p>
          </div>
      </div>
      <div class="text-center">
        <button class="link_btn "> VIEW ALL POSTS</button>
      </div>
  </section>
</template>

<script>
export default {
name:"Blog",
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
.col-3{
    .date, p{
        color:$grey
    }
    h3{
        color:$marino
    }
    img{
        width: 80%;
        border-radius: .3125rem
        
    };
}
    span{
        color:$jungle
    }
h4{
    color:$grey;
    font-size: 1rem;
}
.link_btn{
    background-color: white;
    color: $jungle;
    border: none;
    &:hover{
         box-shadow:none ;
             transform: none;
             text-decoration: 3px  underline;
    }
}
</style>