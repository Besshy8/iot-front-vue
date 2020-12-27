<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Header msg="Jetson Nano REST API"/>
    <RestApi></RestApi>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import RestApi from './components/RestApi.vue'

export default {
  name: 'App',
  components: {
    Header,
    RestApi
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
