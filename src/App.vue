<template>
  <div class="site-bearbot">
    <BearFloat />
  </div>
</template>

<script>
import BearFloat from './components/BearFloaty.vue'

export default {
  name: 'bearbot-app',
  components: {
    BearFloat
  }
}
</script>

<style>
body {
  background-color: #36393e; 
}
</style>
