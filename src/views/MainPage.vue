<script setup>
import { inject } from 'vue'
import HorizontalList from '../components/HorizontalList.vue';

const listCount = inject('getRandomInt')(100, 200)
</script>

<template>
  <div class="main_list">

    <h1 class="main_list__title">OMG_vertical_test</h1>

    <HorizontalList v-for="index in listCount" :key="index"/>

  </div>
</template>

<style scoped lang="scss">
.main_list {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 24px;
}

.main_list__title {
  margin: 24px 0;
}
</style>
