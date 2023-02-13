<template>
  <!-- <div class="container-fluid"> -->
    <div class="row-3">
      <div class="col-6">
        <rigaimg v-for="(immagine, index) in immagini" :key="index" :immagine="immagine"/>
      </div>
      <div class="col-6">
        <rigaimg1 v-for="(immagine2, index) in immagini2" :key="index" :immagine2="immagine2"/>
      </div>
    </div>
  <!-- </div> -->
</template>

<script>
import Fumetti from '@/data/Fumetti.js'
import rigaimg from '@/components/rigaimg.vue'
import rigaimg1 from '@/components/rigaimg1.vue'

export default {
  name: 'HelloWorld',
  components: {
    rigaimg,
    rigaimg1,

  },
  data(){
    return{
      immagini:  Fumetti.filmLinks,
      immagini2:  Fumetti.filmLinksEcond

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.row-3{
  height: 100px;
  width: 100%;
  border: 2px solid black;
  position: absolute;
  top: 70px;
}
</style>
