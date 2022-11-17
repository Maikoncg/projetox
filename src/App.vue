<template>
  <div id="app">
    <LocationCard />
  </div>
</template>

<script>
import LocationCard from './components/LocationCard.vue'

export default {
  name: 'App',
  components: {
    LocationCard
  }
}
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
}
</style>
