<template>
  <div>
    <form @submit="handleSubmit">
      <input type="text" placeholder="Enter something" v-model="inputValue" />
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script setup>
import { ref } from "vue";
const inputValue = ref("");

const handleSubmit = (event) => {
  event.preventDefault();
  console.log("Form submission prevented!");
};
</script>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  width: 200px;
}

input {
  padding: 5px;
}

button {
  padding: 5px;
  cursor: pointer;
}
</style>
