<template>
  <div>
    <img :src="immagine2.thumb" :alt="immagine2.series">
  <!-- <p>{{ immagine }}</p> -->
</div>
</template>

<script>

export default {
  props:[
   "immagine2"

  ],
  name: 'HelloCorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img{
  width: 200px;
}
</style>
