<template>
  <div>
    <img :src="immagine.thumb" :alt="immagine.series">
  <!-- <p>{{ immagine }}</p> -->
</div>
</template>

<script>

export default {
  props:[
   "immagine"

  ],
  name: 'HelloSorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img{
  width: 200px;
}
</style>
