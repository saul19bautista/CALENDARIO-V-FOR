<script setup>
import { ref } from 'vue'

defineProps({
  edad: String,
})
const count = ref(0)
</script>
<template>
<h6>hola soy el componente Hijo2</h6>
<h6>{{ edad }}</h6>
</template>
<style scoped>

</style>
