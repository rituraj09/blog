<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <Home data="Rituraj is here" msg="Hi, from Rituraj"/> -->
  <div id="app">
    <Index />
  </div>
</template>


<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
import Index from "./components/Index";
export default {
  name: "App",
  components: {
    // HelloWorld,
    // Home,
    Index,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50; 
}
</style>
