<template>
  <div id="app">
    <Notifications />
  </div>
</template>

<script>
import Notifications from './components/Notifications'

export default {
  name: 'App',
  components: {
    Notifications
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

body {
  background: #a8cfee;
}

</style>
