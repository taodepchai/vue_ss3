<template>
  <div>
    <a href="http://www.google.com" @click="checkLink">Go to Google</a>
  </div>
</template>

<script setup>
const checkLink = (event) => {
  const url = event.target.href;

  if (!url.startsWith("https://")) {
    event.preventDefault(); 
    alert("Đường dẫn không hợp lệ. Đường dẫn phải bắt đầu với 'https://'");
  }
};
</script>

<style scoped>
a {
  color: blue;
  text-decoration: underline;
  cursor: pointer;
}
</style>
