<template>
  <div class="row-2 g-0">
      <div class="col-12 scrt">
        <span class="scritta">
          <h1>RETURN TO THE WORLD OF INJUSTICE</h1>
          <P>Tom Taylor reveals Adventures of Superman: Jon Kent's massive twist--the miniseries will transport its young hero to the dark world of Injustice.</P>
        </span>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloNorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
.row-2{
  height: 400px;
  width: 100%;
  background-image: url(../assets/jumbotron.jpg);
  background-size:cover;
  background-repeat:no-repeat;
  background-position: left top right;
  
.scrt{
  background-color: rgba(0,0,0,0.6);
  width: 100%;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  .scritta{
    height: 150px;
    width: 67%;
    position: absolute;
    text-align: center;
    color: white;
    h1{
      font-weight:700;
    }
  }
}
}
@media screen and (max-width:1150px){
  
}
</style>
