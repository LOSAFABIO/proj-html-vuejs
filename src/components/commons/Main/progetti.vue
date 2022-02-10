<template>
    <div class="progetti">
      <div class="jumbo-progetti">
        <div v-for="(elemento, indice) in progettiArr" :key="indice" class="progetto">
          <img :src="elemento.image" alt="">
        </div>
        <!-- <div class="progetto">
          <img src="../../studio/img/port-img-08.jpg" alt="">
        </div>
        <div class="progetto">
          <img src="../../studio/img/port-img-09.jpg" alt="">
        </div>
        <div class="progetto">
          <img src="../../studio/img/port-img-10.jpg" alt="">
        </div>
        <div class="progetto">
          <img src="../../studio/img/port-img-11.jpg" alt="">
        </div>
        <div class="progetto">
          <img src="../../studio/img/port-img-12.jpg" alt="">
        </div> -->
      </div>
      <i class="fa-solid fa-caret-right"></i>
      <i class="fa-solid fa-angle-up"></i>
    </div>

</template>

<script>
export default {
    name  : "progetti",
    data() {
        return {
            progettiArr : [
                {
                    image : require("../../../studio/img/port-img-07.jpg") 
                },
                {
                    image : require("../../../studio/img/port-img-08.jpg") 
                },
                {
                    image : require("../../../studio/img/port-img-09.jpg")
                },
                {
                    image : require("../../../studio/img/port-img-10.jpg")
                },
                {
                    image : require("../../../studio/img/port-img-11.jpg") 
                },
                {
                    image : require("../../../studio/img/port-img-12.jpg") 
                }
            ]
        }
  }

}
</script>

<style scoped lang="scss">

.progetti{
    height: 1082px;
    background-image: url("../../../studio/img/h2-background-img-02 (1).png");
    background-repeat: repeat;
    background-size: 85%;
    background-position: 6px;
    position: relative;

    .fa-caret-right{
        bottom: 16%;
    }

    .fa-angle-up{
        bottom: 18.5%
    }


    .jumbo-progetti{
        display: flex;
        flex-wrap: wrap;
        width: 720px;
        margin: -90px auto;

        .progetto{
        height: 360px;
            img{
                width: 360px;
                height: 100%;
            }
        }
    }
}


</style>