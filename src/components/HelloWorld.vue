<template>
    <div class="row-3">
      <div class="col-12 ig1">
        <rigaimg v-for="(immagine, index) in immagini" :key="index" :immagine="immagine"/>
      </div>
      <div class="col-12 ig2">
        <rigaimg1 v-for="(immagine2, index) in immagini2" :key="index" :immagine2="immagine2"/>
      </div>
    </div>
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
<style lang='scss' scoped>
.row-3{
  height: 740px;
  width: 100%;

  background-color: #202328;
.ig1 , .ig2{
  display: flex;
  justify-content: space-around;
  align-items:center;
  height: 360px;
}
}
@media screen and (max-width:768px){
}
@media screen and (max-width:600px){
  .row-3{
    width: 100%;
    height: 100%;
    .ig1{
      border: 2px solid red;
      height: 100%;
      display:contents;
    }
    .ig2{
      // display: none;
      height: 100%;
      display:contents;
    }
  }
}
</style>
