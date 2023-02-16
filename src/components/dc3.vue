<template>
  <div class="row-4">
    <div class="col-1">
      <p>DIGITAL COMIX</p>
    </div>
    <div class="col-1">
      <p>MERCHANDISE</p>
    </div>
    <div class="col-1 ll">
      <img src="../assets/buy-comics-subscriptions[5595].png" alt="">
      <p>SUBSCRIPTIONS</p>
    </div>
    <div class="col-1">
      <img src="../assets/buy-comics-shop-locator[5594].png" alt="">
      <p>SHOP LOCATOR</p>
    </div>
    <div class="col-1">

      <p>POWER VISA</p>
    </div>
  </div>

</template>

<script>
export default {
  name: 'HelloWworld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.row-4{
  height: 80px;
    width: 100%;
    background-color: #0082FA;
    display: flex;
    justify-content: space-around;
  .col-1{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 20%;
  img{
  //  width: ;
  margin-right: 5px;
  margin-top: -5px;
   height: 25px;
  }
  p{
    margin-top: 10px;
    color: white;
  }
}
}
@media screen and (max-width:768px){
}
@media screen and (max-width:600px){
.row-4{
  display: none;
}
}
</style>
