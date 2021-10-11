<template>
  <div id="app">
    <Header :infoNav="linkNav"/>
    <Main/>
    <Footer/>
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
      linkNav:["Home", "Pages", "Courses", "Features", "Blog", "Shop"
      ]
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';

</style>
