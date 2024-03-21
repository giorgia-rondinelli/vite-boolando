<script>
export default {
 
}
</script>

<template>
  <header>
    <div class="fisso">
      <div class="contenitore intestazione">
        <nav>
          <ul>
            <li><a href="">Donna</a></li>
            <li><a href="">Uomo</a></li>
            <li><a href="">Bambini</a></li>
          </ul>
        </nav>
        <div class="logo"><img src="/public/img/boolean-logo.png" alt=""></div>
        <div class="icone">
          <i class="fa-regular fa-user"></i>
          <i class="fa-regular fa-heart"></i>
          <i class="fa-solid fa-bag-shopping"></i>
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
