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
    .col-2
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
</style>
