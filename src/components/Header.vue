<template>
  <div class="container">
    <div class="logo">
      <img class="logo-img" src="../studio/img/logo-img-01.png" alt="">
    </div>
    <nav class="menu">
      <ul class="listamenu">
        <li class="active">
          <a href="#">Home</a>
        </li>
        <li>
          <a href="">Pages</a>        
        </li>
        <li>
          <a href="">Portfolio</a>
        </li>
        <li>
          <a href="">Blog</a>
        </li>
        <li>     
          <a href="">Shop</a>
        </li>
        <li>     
          <a href="">Elements</a>
        </li>
        <li>     
          <a href="">
            <img src="../studio/svg/svg-1.svg" alt="">
          </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}

.logo-img{
  width: 32%;
  margin-left: 10px;
}

.listamenu{
  display: flex;
  justify-content: center;

    li{
      list-style-type: none;
      margin: 10px 20px;
      font-size: 0.8rem;

      a{
        text-decoration: none;
        color: black;

        img{
          width: 15px;
          height: 15px;
        }
      }
    }
}


</style>
