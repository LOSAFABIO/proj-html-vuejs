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
          <a href="">menu</a>
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
  background-color: antiquewhite;
  padding: 10px;
}

.logo-img{
  width: 32%;
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
      }
    }
}


</style>
