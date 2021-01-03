<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" width="60" height="60"><br><br>
 
    <!-- <HelloWorld msg=""/> -->
    <!-- <List msg=""/> -->
    <Movies msg=""/>
    <!-- <Card /> -->
  </div>

</template>

<script>
import Movies from './components/Movies.vue'
// import HelloWorld from './components/HelloWorld.vue'
// import Card from './components/Card'
// import List from './components/List.vue'
 


export default {
  name: 'App',
  components: {
    // HelloWorld,
    // List
    Movies,
    // Card
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
