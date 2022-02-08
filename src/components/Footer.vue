<template>
  <div class="container">
    <div class="text-footer">
      <img class="logo-img" src="../studio/img/logo-img-01.png" alt="">
      <p>Sometimes doing somewthing seemingly demanding turns out to be fun. 
        <br> Here's the proof - Bryson, your brand new portfolio. </p>
      <div class="social-footer">
        <a href="#">
          <img src="" alt="">
        </a>
        <a href="#">
          <img src="" alt="">
        </a>      
        <a href="#">
          <img src="" alt="">
        </a>      
        <a href="#">
          <img src="" alt="">
        </a>      
      </div>
      <i class="fa-solid fa-caret-right"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container{
  background-image: url("../studio/img/h2-footer-img-01.jpg");
  background-position: center; 
  background-repeat: no-repeat;
  background-size: 100%;
  padding: 70px 0 ;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  .text-footer{
    text-align: center;
    font-size: 0.7rem;
  }
  .logo-img{
    width: 22%;
    margin: 10px;
  }
}

</style>
