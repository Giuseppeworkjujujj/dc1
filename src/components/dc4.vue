<template>
  <div class="row-5">
    <div class="col-2 kj">
      <ul class="ones">
        <li><h5>DC COMICS</h5></li>
        <li>Characters</li>
        <li>Comics</li>
        <li>Movies</li>
        <li>Tv</li>
        <li>Games</li>
        <li>News</li>
      </ul>
      <ul class="dose">
        <li><h5>SHOP</h5></li>
        <li>Shop DC</li>
        <li>Shop DC collectibles</li>
      </ul>
    </div>
    <div class="col-2 pk">
      <ul class="tres">
        <li><h5>DC</h5></li>
        <li>Terms Of Use</li>
        <li>Privacy Policy (New)</li>
        <li>Ad Choices</li>
        <li>Advertising</li>
        <li>Jobs</li>
        <li>Subscriptions</li>
        <li>Talent Workshops</li>
        <li>CPSC Certificates</li>
        <li>Ratings</li>
        <li>Shop Help</li>
        <li>Contact Us</li>
      </ul>
    </div>
    <div class="col-2 nk">
      <ul class="quatros">
        <li><h5>SITES</h5></li>
        <li>DC</li>
        <li>MAD Magazine</li>
        <li>DC Kid</li>
        <li>DC Universe</li>
        <li>DC Power Visa</li>
      </ul>
    </div>
    <div class="col-6 jk">

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
.row-5{
  height: 300px;
  width: 100%;
  background-image: url(../assets/footer-bg.jpg);
  background-size:cover;
  background-repeat:no-repeat;
  background-position: left top right;
  display: flex;
  .kj{
    height: 300px;
    width: 20%;
    .ones{
      margin-top: 20px;
      color: gray;
      list-style: none;
      line-height: 20px;
      h5{
        color: white;
      }
    }
    .dose{
      margin-top: 20px;
      color: gray;
      list-style: none;
      line-height: 20px;
      h5{
        color: white;
      }
    }
  }
  .pk{
    width: 20%;
    height: 300px;
    .tres{
      // position: absolute;
      margin-top: 20px;
      color: gray;
      list-style: none;
      line-height: 20px;
      h5{
        color: white;
      }
    }
  }
  .nk{
    height: 300px;
    width: 20%;
    .quatros{
      // position: absolute;
      color: gray;
      margin-top: 20px;
      list-style: none;
      line-height: 20px;
      h5{
        color: white;
      }
    }
  }
  .jk{
  width: 40%;
  height: 300px;
  padding-top: 0px;
  background-image: url(../assets/dc-logo-bg.png);
  background-size:80%;
  background-repeat:no-repeat;
  background-position: left;
  }
}
@media screen and (max-width:768px){
}
@media screen and (max-width:600px){
.row-5{
  display: none;
}
}
</style>
