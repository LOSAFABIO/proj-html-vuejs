<template>
  <div class="container">
    <div class="logo">
      <img class="logo-img" src="../studio/img/logo-img-01.png" alt="">
    </div>
    <nav class="menu">
      <menuHeader />
    </nav>
  </div>
</template>

<script>
import menuHeader from "./commons/Header/menuHeader.vue"

export default {
  name       : 'Header',
  components : {
    menuHeader
  }
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


</style>
