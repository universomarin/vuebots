<template>
  <div>
    <li
      v-for="bot in bots"
      :key="bot.id"
    >
      {{ bot.id }}
    </li>
  </div>
</template>

<script lang="ts">

export default {
  name: 'BotList',
  data: () => ({
    bots: [
      {
        id: 'Bot 1',
        position: { lat: 3, lng: 101 }
      },
      {
        id: 'Bot 2',
        position: { lat: 5, lng: 99 }
      },
      {
        id: 'Bot 3',
        position: { lat: 6, lng: 97 }
      }
    ]
  })
}
</script>
