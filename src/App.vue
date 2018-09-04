<template>
  <div id="app">
    <HelloWorld msg="Scoreboard"/>
    <Greetings user="Mike"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Greetings from './components/Greetings.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Greetings
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
