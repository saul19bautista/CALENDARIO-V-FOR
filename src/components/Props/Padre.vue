<script setup>
import { ref } from 'vue'
import Hijo1 from './Hijo1.vue'
import Hijo2 from './Hijo2.vue'

const count = ref(0)
</script> 
<template>
  <div class="container">
    <h1>hola soy el componente padre</h1>
<Hijo1 class="mt-4" edad="15"/>
<Hijo2 class="mt-4" edad="24"/>
  </div>

</template>
<style scoped>

</style>
