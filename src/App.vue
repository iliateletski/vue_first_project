<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
</template>

<style scoped>
.container {
  max-width: 1232px;
  padding: 23px 78px 12px;
  margin: 0 auto;
  box-shadow: 0px 4px 27px 0px #e6e7eac7;
  min-height: 100%;
  display: flex;
  flex-direction: column;
}

@media (max-width: 740px) {
  .container {
    padding: 23px 40px 12px;
  }
}

@media (max-width: 590px) {
  .container {
    padding: 23px 23px 12px;
  }
}
</style>
