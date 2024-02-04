<script setup>
import Recipe from './views/Recipe.vue';
</script>

<template>
  <div class="container"><Recipe/></div>
</template>

<style scoped>
  .container{
    width: 46%;
    margin: 80px auto;
    background: hsl(0, 0%, 100%);
    border-radius: 20px;
  }

  @media (width <=768px){
    .container{
      width: 100%;
      margin: 0;
      border-radius: 0px;
    }      
  }
</style>
