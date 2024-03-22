<script>
export default {
  props:{
    productImagef: String,
    productImageb: String,
    productBrand: String,
    productName: String,
    productPrice: Number,
    productDiscount: String
    
  }

 
}
</script>

<template>

<div class="card">
        <div class="levi">
          <img :src="`/public/img/${productImagef}`" alt="">
          <img  class="seconda-immagine" :src="`/public/img/${productImageb}`" alt="">
          <div class="cuore nero">&#9829;</div>
          <div class=" etichetta sale half" >-50%</div>
          <div class=" etichetta sostenibilità">Sostenibilità</div>
        </div>
        <div class="marca">{{productBrand}}</div>
        <div class="descrizione">{{productName}}</div>
        <div>
         
          <span class="prezzo originale">{{ productPrice }}&euro;</span>
        </div>
      </div>
  
</template>


<style lang="scss" >
.card{
  width: 30%;
  height:50%;
  position: relative;
  .levi{
    position: relative;
    img{
      width: 100%;
    }
    .seconda-immagine{
      display: block;
      position: absolute;
      top: 0;
    &:hover{
      display: none;
    }
    }
    .cuore{
 
      height: 50px;
      width: 50px;
      position: absolute;
      right: 0;
      top: 5px;
      font-size: 2em;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: white;
      color: black;
    }
    .etichetta{
      color: white;
      font-size: 12px;
      font-weight: 600;
      padding: 5px;
      position: absolute
    }
    .sale{
      background-color: red;
      width:40px;
      left: 0;
      bottom: 30px;
    }
    .sostenibilità{
      background-color: green;
      left: 45px;
      bottom: 30px;
    }
  }
  .marca{
    font-size: 12px;
  }
  .descrizione{
    font-weight: 600;
    font-size:0,8em;
  }
  .prezzo.scontato{
    color: red;
    font-weight: 600;
  }
  .prezzo.originale{
   

  }


 
}

</style>