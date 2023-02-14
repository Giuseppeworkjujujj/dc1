<template>
  <div class="jk">
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
<style lang='scss' scoped>
.jk{
  display: inline;
  img{
    height: 300px;
  }
}
</style>
