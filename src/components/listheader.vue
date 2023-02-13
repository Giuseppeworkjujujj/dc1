<template>
  <div>
    <ul>
    <li :src="lista.text">{{ lista.text }}</li>
  </ul>
  <!-- <p>{{ immagine }}</p> -->
</div>
</template>

<script>

export default {
  props:[
   "lista"

  ],
  name: 'HelloPorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img{
  width: 200px;
}
</style>
