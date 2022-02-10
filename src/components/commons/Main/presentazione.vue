<template>
    <div class="presentazione">
        <div class="jumbo-presentazione">
            <div class="container-titolo">
                <div class="titolo-presentazione">
                    <h1>We are Bryson, New York-based art & design studio</h1>
                </div>
            </div>
            <div class="container-desctizione">
                <div class="descrizione-presentazione">
                    <p>Here at Bryson it only takes a smidgen of imagination and we've already prepared purselves for future challenges. Take a peek and see if you recognize the trademark ingredients of our work </p>
                </div>
            </div>
        </div>
        <div class="arrow">
            <i class="fa-solid fa-caret-right"></i>
            <i class="fa-solid fa-angle-up"></i>
        </div>
    </div>

</template>

<script>
export default {
    name : "presentazione"
}
</script>

<style scoped lang="scss">

.presentazione{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 361px;
  width: 100%;
  margin: 0 0 30px 0;
  background-image: url("../../../studio/img/h2-background-img-02.png");
  background-repeat: repeat;
  background-size: 85%;
  position: relative;

  .fa-caret-right{
    bottom: -130%
  }

  .fa-angle-up{
    bottom: -122.5%
  }

  .jumbo-presentazione{
  display: flex;
  align-items: center;
  width: 70%;
  margin: 0 auto;
  }

  .container-titolo{
    width: 75%;

    .titolo-presentazione{
      width: 90%;
      
      h1{
        font-size: 1.9rem;
        line-height: 1.1;
      }
    }
  }
  .container-desctizione{
    width: 90%;

    .descrizione-presentazione{
      width: 95%;
    }
    p{
      padding: 10px 0;
    }
  }
}


</style>