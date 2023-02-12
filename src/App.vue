<template>
  <div id="app">
    <HelloWorld/>
    <dc1/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import dc1 from './components/dc1.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    dc1,
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
