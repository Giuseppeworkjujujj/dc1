<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 prima-riga">
        <listheader v-for="(lista, index) in liste" :key="index" :lista="lista"/>
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
<style scoped>
  .prima-riga{
    width: 100%;
    height: 70px;
    border: 2px solid red;
    position: relative;
    margin-top: 0px;
  }
</style>
