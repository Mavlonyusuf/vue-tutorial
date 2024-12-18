<template>
  <div>
    <p>{{ sanoq }}</p>
    <button @click="increment">oshirish</button>
    <button @click="increment">kamaytirish</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
let sanoq = ref(0);
function increment() {
  sanoq.value++;
}
</script>

<style scoped>
button {
  background-color: darkgreen;
  color: white;
  padding: 11px 33px;
  border: 1px solid transparent;
  border-radius: 8px;
  cursor: pointer;
}
</style>
