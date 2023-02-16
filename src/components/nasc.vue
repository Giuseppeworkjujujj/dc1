<template>
  <span class="ssss">
    <button class="ret btn btn-white" @click="hideOrShow">{{ buttonLabel }}</button>

    <!-- <div class="row-n "  > -->
      <div class="col-md-12 qq" v-if="isVisible" >
        <navbar v-for="(nav, index) in liste" :nav="nav" :key="index" />
      </div>
    <!-- </div> -->
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
      isVisible: false

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
.ret{
  display: none;
}
.qq{
  border: 2px solid blue;
}

@media screen and (max-width:768px){
  .ret{
    display: flex;
    position: absolute;
    top: 50px;
    right: 5px;
    transition:all 40ms ease-in-out;
    border: 2px solid #0082FA;
    color: #0082FA;
  }
  // .row-n{
  //   display: flex;
    // overflow: hidden;
    // position: absolute;
    // background-color: white;
    // width: 100%;
    // height: 70px;
    // border: 2px solid red;
    // line-height: 5px;
.qq{
  width: 100%;
  position:absolute;
  overflow: hidden;
  z-index: 1;
  background-color: white;
  // transition-duration:all 40ms ease-in;
    // transition-duration: 2s;
    // transition-timing-function: 2s;}
  // }
}}
</style>
