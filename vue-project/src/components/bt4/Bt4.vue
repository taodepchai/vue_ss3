<template>
  <div>
    <div
      :class="{ active: isActive }"
      :style="{ backgroundColor: backgroundColor }"
      class="block"
    >
      Block
    </div>
    <p>isActive={{ isActive }}</p>
  </div>
</template>

<script setup>
const isActive = true;
const backgroundColor = "blue";
</script>

<style scoped>
.block {
  width: 200px;
  height: 100px;
  text-align: center;
  line-height: 100px;
  color: black;
  margin-bottom: 10px;
}

.active {
  color: #fff; /* Đổi màu chữ khi isActive là true */
}
</style>
