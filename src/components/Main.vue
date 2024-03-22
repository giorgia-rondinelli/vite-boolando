<script>
import Card from './partials/Card.vue'
import {products} from '../assets/db.json'


export default {
  components:{
    Card,
    
  },
  data(){
    return{
      products
    }
  }
  

  
 
  

 

 
}
</script>

<template>
   <main>
    <div class="contenitore principale"> 
      <Card 
      v-for="(product, index) in products"
      :key="index"
      :productImagef="`../../public/img/${product.frontImage}`"
      :productImageb="`../../public/img/${product.backImage}`"
      :productBrand="product.brand"
      :productName="product.name"
      :productPrice="product.price"
     
      
    
      
    
  
     
      />
     
    </div>
  </main>

</template>

<style scoped>



.principale{
  height: 1300px;
  padding-top: 100px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between

}

</style>
