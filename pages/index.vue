<template>
  <div class="content">
    <MapIndex class="map" />
    <BotList />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
</script>

<style scoped>
  .content {
    display: flex;
  }
  .map {
    height: 400px;
  }
</style>
