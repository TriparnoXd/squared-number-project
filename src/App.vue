<script setup>
  import {ref, computed} from 'vue'
  const number = ref(5);

  const squaredNumber = computed(()=>number.value*number.value)

  
</script>

<template>
  <h1 class="number">The number is : {{ number }}</h1>
  <button @click="()=>number++">Increase</button>
  <button @click="()=>number--">Decrease</button>
  <button @click="()=>number=0">Default</button>
  <h1 class="squared">The sqaure of the number is : {{ squaredNumber }}</h1>
  
</template>

<style scoped>
  button{
    margin: 10px
  }
</style>