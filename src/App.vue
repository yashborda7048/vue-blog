<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!--Here, This data is coming from home.vue component as such import -->
    <Home data="Yes you are here and also started work with vue" msg="You must need to focus with vue"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // It is also we have defined when we create a new component
    Home
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
