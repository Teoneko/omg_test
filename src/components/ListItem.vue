<script setup>
const productNumber = Math.floor(Math.random() * Math.floor(1000))
</script>

<template>
  <div class="list_item">{{ productNumber }}</div>
</template>

<style scoped lang="scss">
.list_item {
  display: flex;
  align-items: center;
  justify-content: center;
  border: 2px solid #618e99;
  border-radius: 10px;
  overflow: hidden;
  padding: 5px 10px;
  margin-right: 10px;
  min-width: min-content;
  transition: all .3s ease-in-out;
  margin-bottom: 5px;
  cursor: pointer;
}

.list_item:hover {
  transform: scale(0.8);
}
</style>
