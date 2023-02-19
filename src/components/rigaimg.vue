<template>
  <div class="jk">
    <img :src="immagine.thumb" :alt="immagine.series">
  <!-- <p>{{ immagine }}</p> -->
</div>
</template>

<script>

export default {
  props:[
   "immagine"

  ],
  name: 'HelloSorld',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.jk{
  display: inline;
  img{
    height: 300px;
  }
}
@media screen and (max-width:890px){
  .jk{
    // border: 2px solid blue;
    height: 300px;
    width: 200px;
    margin-top: 25px;
    margin-bottom: 20px;
  img{
    // border: 2px solid yellow;
    height: 300px;
  }
  }

}
@media screen and (max-width:600px){
  .jk{
    display:flex;
    justify-content: center;
    margin-top: 0px;
    margin-bottom: 0px;
    width: 100%;
    height: 100%;
  img{
    height: 300px;
    border-radius: 10%;
    margin:50px;
    transition: 0.3s ease;
    -moz-transition: 0.3 ease; /* Firefox */
    -webkit-transition: 0.3s ease; /* Chrome - Safari */
    -o-transition: 0.3s ease; /* Opera */
  }
  img:hover{
    transform : scale(1.2);
    -moz-transform : scale(1.2); /* Firefox */
    -webkit-transform : scale(1.2); /* Chrome - Safari */
    -o-transform : scale(1.2); /* Opera */
  }
  }
}
</style>
