<template>
  <div id="app">
    <Header :infoNav="linkNav" :infoMed="media" :infoShop="shop"/>
    <Main/>
    <Footer :infoMed="media" :infoLinkFooter="footerLink"/>
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'



export default {
  name: 'App',
  components: {
    Main,
    Footer,
    Header,
  },
  data(){
    return{
      linkNav:["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
      media:["fa-twitter", "fa-facebook-f", "fa-instagram", "fa-linkedin"],
      shop:["far fa-caret-square-right", " far fa-life-ring"," fas fa-book","fas fa-shopping-cart"],
      footerLink:[
        {
          title:"Titolo-1",
          link:["link1", "link2", "link3"]
        },
          {
          title:"Titolo-2",
          link:["link1", "link2", "link3"]

        }

      ],
      
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';

</style>
