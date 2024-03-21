<script>
export default {
 
}
</script>
<template>
   <footer>
    <div class="foot contenitore ">
      <div class="informazioni">
        <h5>Boolando s.r.l</h5>
        <div>
          <span>Informazioni legali</span>
          <span>Informativa sulla privacy</span>
          <span>Diritto di recesso</span>
        </div>
      </div>
      <div class="social">
        <h6>Trovaci anche su</h6>
        <div>
          <i class="fa-brands fa-square-twitter"></i>
          <i class="fa-brands fa-square-facebook"></i>
          <i class="fa-brands fa-square-instagram"></i>
          <i class="fa-brands fa-square-pinterest"></i>
          <i class="fa-brands fa-youtube"></i>
        </div>
      </div>
  </div>
  </footer>

</template>

<style lang="scss" scoped>

@use "../assets/scss/partial/variables.scss" as*;

footer{
  height: 70px;
  background-color:$bg-footer;
  color:$text-white;
  .foot{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    h5{
      font-size: .9rem;
    }
    span{
      font-size: .7em;
      margin-right: 5px;
    }
    div{
      margin-top: 8px;
      i{
        margin-right: 5px;
      }
      
    }

  }
}


</style>