<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Home1 />
    <Home />
  </div>
</template>

<script>
import Home1 from "./pages/Home1"
import Home from "./pages/Home"
export default {
  name: 'App',
  components: {
    Home1,Home
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
