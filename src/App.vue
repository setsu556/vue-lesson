<script setup>
import { ref } from 'vue'
const title = ref('Vue.js Course')
let price = ref(9.99)
function increment() {
  price.value += 1
}
const info = ref({
  students: 1000,
  rating: 4,
})
console.log(info.value.students)
</script>
<template>
  <h1>Title: {{ title }}</h1>
  <h2>Price: ${{ price - 1 }}</h2>
  <button @click="increment">button</button>
  <h2>Students: {{ info.students }}</h2>
</template>
