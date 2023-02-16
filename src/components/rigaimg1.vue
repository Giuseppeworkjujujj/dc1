<template>
  <div class="jj">
    <img :src="immagine2.thumb" :alt="immagine2.series">
  <!-- <p>{{ immagine }}</p> -->
</div>
</template>

<script>

export default {
  props:[
   "immagine2"

  ],
  name: 'HelloCorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.jj{
  display: inline;
  img{
    height: 300px;
  }
}
@media screen and (max-width:768px){
}
@media screen and (max-width:600px){
  .jj{
    display:flex;
    justify-content: center;
    // border: 2px solid blue;
  img{
    // border: 2px solid red;
    height: 300px;
    border-radius: 10%;
    margin:50px;
    transition: 0.3s ease;
    -moz-transition: 0.3 ease; /* Firefox */
    -webkit-transition: 0.3s ease; /* Chrome - Safari */
    -o-transition: 0.3s ease; /* Opera */
    // -ms-transform : 1.2s ease; /* IE */
  }
  img:hover{
    transform : scale(1.2);
    -moz-transform : scale(1.2); /* Firefox */
    -webkit-transform : scale(1.2); /* Chrome - Safari */
    -o-transform : scale(1.2); /* Opera */
    // -ms-transform : scale(1.3); /* IE */
  }
  }
}
</style>
