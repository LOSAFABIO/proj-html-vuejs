<template>
    <div class="video">
        <a href="#">
            <img src="../../../studio/img/main-home-video-button-img-01.png" alt="">
        </a>
        <i class="fa-solid fa-caret-right"></i>
        <i class="fa-solid fa-angle-up"></i>
    </div>
</template>

<script>
export default {
    name : "videoProject"
}
</script>

<style scoped lang="scss">

.video{
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url("../../../studio/img/h2-img-2.jpg");
  background-size: 85%;
  background-position:center;
  height: 350px;
  position: relative;

  .fa-caret-right{
    bottom: 45%;
  }

  .fa-angle-up{
      bottom: 52.5%
    }

  img{
    width: 60px;
    &:hover{
      opacity: 0.9;
    }
  }
}


</style>