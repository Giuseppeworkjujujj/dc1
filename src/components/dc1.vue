<template>
  <div class="container-fluid">
    <div class="row-2">
      <div class="col-6 seconda-riga">
        <img src="../" alt="">
      </div>
      <div class="col-6 prima-riga">
        <listheader v-for="(lista, index) in liste" :lista="lista" :key="index" />
      </div>
    </div>
  </div>
</template>

<script>
import Fumetti from '@/data/Fumetti.js'
import listheader from '@/components/listheader.vue'

export default {
  name: 'HelloNorld',
  components: {
    listheader,
  },
  data(){
    return{
      liste: Fumetti.headerLinks
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.row-2{
  position: relative;
.seconda-riga{
  border: 2px solid blue;
  height: 70px;
  float: left;
  width: 70%;
}
  .prima-riga{
    width: 30%;
    height: 70px;
    border: 2px solid red;
    /* position: relative; */
    margin-top: 0px;
    display: inline-flex;
    float: right;
    
  }
}
</style>
