<template>
  <div v-if="GStore.organizers">
    <div id="nav">
      <router-link :to="{ name: 'organizerDetail' }">Details</router-link>
    </div>
    <router-view :organizer="GStore.organizers" />
  </div>
</template>
<script>
export default {
  inject: ['GStore']
}
</script>
