<template>
  <GoogleMapLoader
    api-key="AIzaSyANpV5T4YdyIJ30-N0s3Ca0U8TfRm1Vp7s"
  />
</template>

<script lang="ts">
import GoogleMapLoader from './GoogleMapLoader.vue'

export default {
  name: 'MapIndex',
  components: {
    GoogleMapLoader
  }
}
</script>
