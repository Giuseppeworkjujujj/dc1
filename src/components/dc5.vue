<template>
  <div class="row-6">
    <div class="col-6 iu">
      <button  class="btn btn-dark">SING-UP NOW!</button>
    </div>
    <div class="col-4 ui">
      <img src="../assets/footer-facebook.png" alt="">
      <img src="../assets/footer-twitter.png" alt="">
      <img src="../assets/footer-youtube.png" alt="">
      <img src="../assets/footer-pinterest.png" alt="">
      <img src="../assets/footer-periscope.png" alt="">
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'HelloSworld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.row-6{
  height: 90px;
  width: 100%;
  display: flex;
  background-color: #202328;
.iu{
height: 90px;
display: flex;
justify-content: center;
align-items: center;
button{
  border: 2px solid #0082FA;
  height: 50px;
}
}
.ui{
  height: 90px;
  display:flex;
  justify-content: space-around;
  align-items: center;
img{
  height: 30px;
}
}
}
@media screen and (max-width:890px){
  .row-6{
    .iu{
      display: none;
    }
    .ui{
      width: 100%;
    }
  }
}
@media screen and (max-width:600px){
.row-6{
  display: flex;
  justify-content: center;
  .iu{
    display: none;
  }
  .ui{
    width: 80%;
    .img{
    transition: 0.5s ease;
    -moz-transition: 0.5s ease; /* Firefox */
    -webkit-transition: 0.5s ease; /* Chrome - Safari */
    -o-transition: 0.5s ease; /* Opera */
    // -ms-transform : 1.2s ease; /* IE */
  }
  img:hover{
    transform : scale(1.9);
    -moz-transform : scale(1.9); /* Firefox */
    -webkit-transform : scale(1.9); /* Chrome - Safari */
    -o-transform : scale(1.9); /* Opera */
    // -ms-transform : scale(1.3); /* IE */
  }
  }
}
}
</style>
