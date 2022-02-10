<template>
    <div class="datiUtente">
        <div class="container-testo-dati">
            <div class="testo-dati">
                <h1>Get in touch and say hello</h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quaerat, quos voluptatem aspernatur.
                    <br> Possimus, beatae!.  </p>
            </div>
        </div>
      <div class="container-inserimento-dati">
            <div class="inserimento-dati">
                <div class="input-testo"><input type="text" placeholder="Comment"></div>
                <div class="input-testo name"><input type="text" placeholder="Name"></div>
                <div class="input-testo email"><input type="text" placeholder="Email"></div>
                <button @click="scrollToTop()">
                    <span>Submit</span>
                    <i class="fa-solid fa-play"></i>
                </button>
            </div>
      </div>
      <i class="fa-solid fa-caret-right"></i>
      <i class="fa-solid fa-angle-up"></i>
    </div>

</template>

<script>
export default {
    name : "datiUtente",
    methods : {
      scrollToTop(){
        window.scrollTo(0, 0);
      }
    }
}
</script>

<style scoped lang="scss">

.datiUtente{
  display: flex;
  height: 160px;
  margin: 80px 0;
  position: relative;

  .fa-caret-right{
    bottom: 85%;
  }

  .fa-angle-up{
    bottom: 101%;
  }

  .container-testo-dati{
    width: 50%;
    position: relative;

    .testo-dati{
      width: 43%;
      position: absolute;
      right: 50px;
    }

    h1{
      font-size: 2.3rem;
      line-height: 1.1;
    }

    p{
      margin: 10px 0;
      width: 300px;
    }
  }
  .container-inserimento-dati{
    width: 50%;
    position: relative;
    margin: -40px 0;

    .inserimento-dati{
      width: 398px;
      position: absolute;
      left: 50px;
    }
    
    .input-testo{
      margin: 40px 0 0 15px;
    }

    .name,.email{
      display: inline-block;
    }
  }
}


</style>