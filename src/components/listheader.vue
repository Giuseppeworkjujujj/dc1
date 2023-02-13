<template>
  <div class="col-6 j1 ">
    <ul src="lista.text"><li class="listato">{{ lista.text }}  </li></ul>
  <!-- <p>{{ immagine }}</p> -->
</div>
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
.j1{
  display: flex;
  justify-content: center;
  align-items: center;
  .listato{
    display: inline;
    list-style: none;
    // float: inline-end;
    // float:inline-start;
    margin-right: 15px;
    height: 20px;
    padding-left: 10px;
  }
}
</style>
