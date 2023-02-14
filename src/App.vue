<template>
  <div id="app">
    <dc1/>
    <dc2/>
    <HelloWorld/>
    <dc3/>
    <dc4/>
  </div>
</template>

<script>
import dc1 from './components/dc1.vue'
import dc2 from './components/dc2.vue'
import HelloWorld from './components/HelloWorld.vue'
import dc3 from './components/dc3.vue'
import dc4 from './components/dc4.vue'
import '@fortawesome/fontawesome-free/css/all.css'
import '@fortawesome/fontawesome-free/js/all.js'
import 'bootstrap/dist/css/bootstrap.min.css'

export default {
  name: 'App',
  components: {
    dc1,
    dc2,
    HelloWorld,
    dc3,
    dc4,
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
