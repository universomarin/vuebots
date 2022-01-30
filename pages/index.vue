<template>
  <div>
    <h1>Map</h1>
    <MapIndex class="map" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
</script>

<style scoped>
  .map {
    height: 400px;
  }
</style>
