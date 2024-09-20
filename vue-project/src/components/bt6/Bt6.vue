<template>
  <div>
    <button @click="handleClick('Rikkei Academy')">Get param</button>
  </div>
</template>

<script setup>
const handleClick = (param) => {
  console.log(param);
};
</script>

<style scoped>
button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}
</style>
