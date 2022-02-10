<template>
  <div class="container">
    <div class="text-footer">
      <img class="logo-img" src="../studio/img/logo-img-01.png" alt="">
      <p>Sometimes doing somewthing seemingly demanding turns out to be fun. 
        <br> Here's the proof - Bryson, your brand new portfolio. </p>
      <div class="social-footer">
        <a href="#">
          <i class="fa-brands fa-instagram"></i>
        </a>
        <a href="#">
          <i class="fa-brands fa-facebook-f"></i>
        </a>      
        <a href="#">
          <i class="fa-brands fa-twitter"></i>
        </a>      
        <a href="#">
          <i class="fa-brands fa-pinterest-p"></i>           
        </a>      
      </div>
      <i class="fa-solid fa-caret-right"></i>
      <i class="fa-solid fa-angle-up"></i>
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

  .fa-angle-up{
    bottom: 9%;
  }

  .social-footer{
    margin: 20px 0;

  a{
    .fa-instagram, .fa-facebook-f, .fa-twitter , .fa-pinterest-p{
          width: 8px;
          height: 8px;
          color: white;
          margin:0 4px;
          background-color: black;
          padding: 6px;
          border-radius: 50%;
      }
      .fa-instagram{
        background-color: #6aa9aa;
      }
      .fa-facebook-f{
        background-color: #f6d193;
      }
      .fa-twitter{
        background-color: #f7bba7;
      }
      .fa-pinterest-p{
        background-color: #d8d496;
      }
    }   
  }
}


</style>
