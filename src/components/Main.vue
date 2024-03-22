<script>
import Card from './partials/Card.vue'

export default {
  components:{
    Card
  }

 
}
</script>

<template>
   <main>
    <div class="contenitore principale"> 
      <Card />
    </div>
  </main>

</template>

<style scoped>

@use "../assets/scss/partial/variables.scss" as*;

.principale{
  height: 1300px;
  padding-top: 100px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between

}

</style>
