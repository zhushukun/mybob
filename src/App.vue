<template>
  <h1>Welcome to Your Vue.js App</h1>
  <img v-if="imageUrl" :src="imageUrl" alt="logo" />
</template>
<script setup>
import { ref } from "vue";
import axios from "axios";

const imageUrl = ref("");
axios.get("dev/api/breeds/image/random").then((res) => {
  let data = res.data;
  console.log(data);
  imageUrl.value = data.message;
});
</script>

<style scoped></style>
