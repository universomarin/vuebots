<template>
  <GoogleMapLoader
    :map-config="mapConfig"
    api-key="AIzaSyANpV5T4YdyIJ30-N0s3Ca0U8TfRm1Vp7s"
    class="google-map"
  >
    <template slot-scope="{ google, map }">
      <GoogleMapMarker
        v-for="marker in markers"
        :key="marker.id"
        :marker="marker"
        :google="google"
        :map="map"
      />
      <GoogleMapLine
        v-for="line in lines"
        :key="line.id"
        :path.sync="line.path"
        :google="google"
        :map="map"
      />
    </template>
  </GoogleMapLoader>
</template>

<script lang="ts">
import { mapSettings } from '../constants/mapSettings'
import GoogleMapLoader from './GoogleMapLoader.vue'

export default {
  name: 'MapIndex',
  components: {
    GoogleMapLoader
  },
  data: () => ({
    markers: [
      {
        id: 'a',
        position: { lat: 3, lng: 101 }
      },
      {
        id: 'b',
        position: { lat: 5, lng: 99 }
      },
      {
        id: 'c',
        position: { lat: 6, lng: 97 }
      }
    ],
    lines: [
      {
        id: '1',
        path: [
          { lat: 3, lng: 101 },
          { lat: 5, lng: 99 }
        ]
      },
      {
        id: '2',
        path: [
          { lat: 5, lng: 99 },
          { lat: 6, lng: 97 }
        ]
      }
    ]
  }),

  computed: {
    mapConfig () {
      return {
        ...mapSettings,
        center: this.mapCenter
      }
    },

    mapCenter () {
      return this.markers[1].position
    }
  }
}
</script>

<style>
  .google-map {
    height: 400px;
    width: 100%;
  }
</style>
