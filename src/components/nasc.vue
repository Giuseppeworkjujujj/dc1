<template>
  <span class="ssss">
    <button class="ret" @click="hideOrShow">{{ buttonLabel }}</button>

    <div class="row-n " v-if="isVisible">
      <div class="col-md-12 qq" >
        <navbar v-for="(nav, index) in liste" :nav="nav" :key="index" />
      </div>
    </div>
  </span>
</template>

<script>
import Fumetti from '@/data/Fumetti.js'
import navbar from '@/components/navbar.vue'

export default {
  name: 'HelloNorld',
  components: {
    navbar,
  },
  data(){
    return{
      liste: Fumetti.headerLinks,
      isVisible: true

    };
  },
  computed: {
  buttonLabel() {
    return this.isVisible ? 'Cerca' : 'Cerca';
  }
},
  methods: {
hideOrShow() {
  this.isVisible = !this.isVisible;
}
}}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>


@media screen and (max-width:768px){
  .ret{
    position: absolute;
    top: 0px;
    right: 5px;
  }
  .row-n{
    display: flex;

.qq{
  border: 2px solid green;
  width: 100%;

}
  }
}
</style>
