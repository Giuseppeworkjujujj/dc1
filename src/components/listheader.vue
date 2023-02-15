<template>
<ul class="topo" src="lista.text"><li class="listato">{{ lista.text }}  </li></ul>
</template>

<script>

export default {
  props:[
   "lista"

  ],
  name: 'HelloPorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>

  .listato{
    display: inline;
    list-style: none;
    height: 20px;
    padding-left: 0px;
  }
  @media screen and (max-width:768px){
  .topo{
    // width: 100%;
    border: 2px solid blue;
  //   display: flex;
  //   justify-content: center;
  // align-items: flex-start;
    display: none;
  .listato{
    display: none;  border: 2px solid red;
  // display: flex;
  // justify-content: center;
  // align-items: flex-start;
  }
}
  }
</style>
