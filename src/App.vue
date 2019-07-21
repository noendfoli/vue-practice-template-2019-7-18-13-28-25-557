<template>
  <div id="app">
    <lastvue></lastvue>
  </div>
</template>

<script>
import lastvue from './components/last.vue'
export default {
  name: 'app',
  components: {
    lastvue
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
