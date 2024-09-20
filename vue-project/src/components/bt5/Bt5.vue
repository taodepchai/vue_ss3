<template>
  <div>
    <button @click="handleClick">Click me</button>
  </div>
</template>

<script setup>
const handleClick = () => {
  console.log("Clicked");
};
</script>

<style scoped>
button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}
</style>
