<template>
  <span class="riga">
  <div class="row-f">
    <div class="col-12 ff nascondi" id="contenuto" src="nac.text">{{ nav.text }}</div>
  </div>
</span>
</template>

<script >
export default {
  props:[
   "nav",
  ],
  name: 'HelloAorld',
  
  data(){
    return{
    }
  },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
  .ret{
    position: absolute;
    top: 0px;
    right: 5px;
    
  }
.row-f{
  width: 100%;
  height: 35px;
.ff{
  text-align: center;
}
}
.ff:hover{
  background-color: gray;
}

  @media screen and (max-width:768px){
  }
</style>
