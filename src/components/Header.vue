<script>
export default {
  data(){
    return{
      menu:[
        'Donna','Uomo','Bambini'
      ],
      icone:[
        {
         
          icona:'<i class="fa-regular fa-user"></i>'

        },
        {
          icona:'<i class="fa-regular fa-heart"></i>'

        },
        {
          icona:'<i class="fa-solid fa-bag-shopping"></i>'

        },

      ]
    }
  }
 
}
</script>

<template>
  <header>
    <div class="fisso">
      <div class="contenitore intestazione">
        <nav>
          <ul>
            <li><a v-for="(item,index ) in menu" href="" :key="index">{{ item }}</a></li>
          
          </ul>
        </nav>
        <div class="logo"><img src="/img/boolean-logo.png" alt=""></div>
        <div  class="icone" :key="index">
          <ul>
            <li><a href="" v-html="icon.icona " v-for="(icon,index ) in icone" :key="index"></a></li>
          </ul>
        
        </div>
      </div>
    </div>
  </header>


</template>

<style lang="scss" scoped>
@use "../assets/scss/partial/variables.scss" as*;

header{
  margin-bottom:40px;
  display:flex ;
  justify-content:center;
  .fisso{
  position:fixed ;
      background-color:$bg-header ;
      width: 100%;
      z-index: 1;
    .intestazione{
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      ul{
        list-style: none;
        display: flex;
        a{
          color:$text-white;
          text-decoration: none;
          font-size: 12px;
          font-weight: 600;
          margin-right: 4px;
        }
      }
      img{
        height: 25px;
      }
      .icone{
        color:$text-white;
        font-size: 12px;
        i{
          padding: 3px
        }
      }
    } 
  }
}


</style>
