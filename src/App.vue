<template>
  <div id="app">
    <h3>Supertext in app</h3>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld />
    <DataComponent />
    <Condition />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import DataComponent from './components/DataComponent.vue'
import Condition from './components/Condition.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    DataComponent,
    Condition,
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
