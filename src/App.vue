<script setup>
import { provide } from 'vue'
import MainPage from './views/MainPage.vue'

const getRandomInt = (min, max) => {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
provide('getRandomInt', getRandomInt);
</script>

<template>
  <MainPage />
</template>
