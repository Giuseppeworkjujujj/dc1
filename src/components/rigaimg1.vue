<template>
  <div class="jj">
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
<style lang='scss' scoped>
.jj{
  display: inline;
  img{
    height: 250px;
  }
}
</style>
