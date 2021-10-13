<template>
    <footer>
        <div class="container">
            <div class="row d-flex align-items-center">
                <div class="col-4">
                    <h4 class="my-3">Address</h4>
                    <div class="address my-5"> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolore tempora inventore itaque vero odio voluptates et quos sit natus. Nihil architecto iure numquam omnis asperiores nulla aliquam eius sequi mollitia.</div>
                    <div  class="icons d-flex my-5"> 
                    <div v-for ="(icon, index) in infoMed" :key="index">
                    <a href="#"> <i :class= "`fab ${icon}`"></i></a>                  
                    </div>
                </div>
                </div>
                <div class="col-8 gx-5 ">
                    <div class="row ">
                        <div class="section_left d-flex ">
                            <div v-for="(obj, index) in infoLinkFooter" :key="index" class="colonna mx-5 text-center">

                            <h4>{{obj.title}}</h4>
                            <div class="list  ">
                            <ul v-for="(link, i) in obj.link" :key="i">
                             <li>{{link}}</li>
                            </ul>
                            
                          

                            </div>
                            </div>
                        
                        </div>
                    
                        
                    </div>
                </div>
            </div>
            <div class="cop text-center py-5">Lorem ipsum dolor sit, amet consectetur adipisicing elit.</div>
        </div>
    </footer>
</template>

<script>
export default {
    name:"Footer",
    props:{
       infoMed:Array,
       infoLinkFooter:Object,
    }
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
footer{
    color: white;
    background-color:$darkBlue;
   
    li, .address, i{
        margin-top: .625rem;
        list-style: none ;
        color:$grey;
    }
    .section_left{
        padding-left:12.5rem;
    }
}
</style>