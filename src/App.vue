<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <StartPage />
  </div>
</template>

<script>
import StartPage from './components/StartPage.vue'

export default {
  name: 'app',
  components: {
    StartPage
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
