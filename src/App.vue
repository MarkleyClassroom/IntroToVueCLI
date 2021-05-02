<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Count msg=" the Dogs">Create a Dog</Count>
    <Count msg=" the Cats">Create a Cat</Count>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Count from './components/Count.vue'
import 'bootstrap'


export default {
  name: 'App',
  components: {
    HelloWorld,
    Count
  }
}
</script>

<style>

* {
  margin:0px;
  padding:0px; 
}

</style>
