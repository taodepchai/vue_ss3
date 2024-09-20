<template>
  <div>
    <button @click="incrementCount">Click me</button>
    <p>Count: {{ count }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const count = ref(0);

const incrementCount = () => {
  count.value++;
};
</script>

<style scoped>
button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}

p {
  font-size: 18px;
}
</style>
