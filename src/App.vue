<script >
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import products from './assets/db.json'
export default { 
  components:{
      Header,
      Main,
      Footer,
      
  },
  data(){
    return{
      products
    }
  }
 

 
  
 
}
 



</script>

<template>
  <div>
  <Header />
  <Main />
  <Footer />
  </div>

  

</template>

<style lang="scss" >
 @use "./assets/scss/main.scss"

</style>
