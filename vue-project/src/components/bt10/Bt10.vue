<template>
  <div>
    <input 
      type="text" 
      v-model="inputText" 
      @keydown.enter="handleEnter"
      placeholder="Nhập văn bản và nhấn Shift + Enter" 
    />
  </div>
</template>

<script setup>
import { ref } from 'vue';

const inputText = ref('');

const handleEnter = (event) => {
  if (event.shiftKey) {
    if (inputText.value.trim()) {
      alert(inputText.value); 
      inputText.value = ''; 
    }
  } else {
    alert("Bạn cần nhấn Shift + Enter");
  }
};
</script>

<style scoped>
input {
  padding: 10px;
  font-size: 16px;
  width: 300px;
}
</style>
