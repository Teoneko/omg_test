<script setup>
import { inject } from 'vue'
import ListItem from './ListItem.vue';

const listCount = inject('getRandomInt')(10, 20)
</script>

<template>
  <div class="horizontal_list">
    <ListItem v-for="index in listCount" :key="index"/>
  </div>
</template>

<style scoped lang="scss">
.horizontal_list {
  width: 100%;
  display: flex;
  margin-bottom: 16px;
  overflow: auto;
}

.horizontal_list::-webkit-scrollbar {
  width: 10px;
  height: 5px;
}

.horizontal_list::-webkit-scrollbar-thumb {
  background: linear-gradient(to bottom right, #4d7fff 0%, #1b55f49e 100%);
  border-radius: 5px;
}
</style>
