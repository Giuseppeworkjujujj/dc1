<template>
  <!-- <div class="col"> -->
    <ul src="lista.text"><li class="listato">{{ lista.text }}  </li></ul>
<!-- </div> -->
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
</style>
