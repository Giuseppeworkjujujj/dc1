<template>
    <div class="row-1 ">
      <div class="col-7 d-flex align-items-center seconda-riga">
        <img src="../assets/dc-logo.png" alt="">
      </div>
      <div class="col-5 prima-riga d-flex justify-content-start align-items-center">
        <listheader v-for="(lista, index) in liste" :lista="lista" :key="index" />
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

.row-1{
  height: 70px;
.seconda-riga{
  height: 70px;
  float: left;
  img{
    width: 60px;
    margin-left: 20px;
  }
}
  .prima-riga{
    height: 70px;
  }
}
</style>
