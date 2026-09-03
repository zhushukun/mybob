<template>
  <h1>github actions deploy</h1>
  <h1>github pages deploy</h1>
  <img v-if="imageUrl" :src="imageUrl" alt="logo" />
</template>
<script setup>
import { ref } from "vue";
import axios from "axios";

const imageUrl = ref("");
axios.get("https://dog.ceo/api/breeds/image/random").then((res) => {
  let data = res.data;
  console.log(data);
  imageUrl.value = data.message;
});
</script>

<style scoped></style>
