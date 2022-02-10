<template>
    <div class="container-tariffe">
        <div class="tariffe">
            <div v-for="(elemento, indice) in tariffeArr" :key="indice" class="tariffa basic">
                <h3>{{elemento.tipo}}</h3>
                <p class="money">{{elemento.costo}}
                    <span class="dollaro">$</span>
                </p>
                
                <ul>
                    <li>
                        <p>{{elemento.concepts}} Design concepts</p>
                    </li>
                    <li>
                        <p>{{elemento.copyright}} copyright ownership</p>
                    </li>
                    <li>
                        <p>{{elemento.direction}} direction</p>
                    </li>
                    <li>
                        <p>{{elemento.creatives}} creatives</p>
                    </li>
                    <li>
                        <p>{{elemento.moneyback}} Money back</p>
                    </li>
                </ul>
                <button @click="scrollToTop()">
                <span>Learn more</span>
                <i class="fa-solid fa-play"></i>
                </button>
            </div>

            <!-- <div class="tariffa standard">
                <h3>Standard</h3>
                <p class="money"> 119$</p>
                <ul>
                    <li>
                        <p>10 Design concepts</p>
                    </li>
                    <li>
                        <p>Full copyright ownership</p>
                    </li>
                    <li>
                        <p>Art direction</p>
                    </li>
                    <li>
                        <p>Top leven creatives</p>
                    </li>
                    <li>
                        <p>No money back</p>
                    </li>
                </ul>
                <button>
                <span>Learn more</span>
                <i class="fa-solid fa-play"></i>
                </button>
            </div>

            <div class="tariffa basic">
                <h3>Basic</h3>
                <p class="money"> 139$</p>
                <ul>
                    <li>
                        <p>15 Design concepts</p>
                    </li>
                    <li>
                        <p>Full copyright ownership</p>
                    </li>
                    <li>
                        <p>Art direction</p>
                    </li>
                    <li>
                        <p>Top leven creatives</p>
                    </li>
                    <li>
                        <p>No money back</p>
                    </li>
                </ul>
                <button>
                <span>Learn more</span>
                <i class="fa-solid fa-play"></i>
                </button>
            </div> -->
        </div>
        <i class="fa-solid fa-caret-right"></i>
        <i class="fa-solid fa-angle-up"></i>
        <div class="img-tariffe">
        <a href="#">
            <img class="circle" src="../../../studio/svg/svg-2.svg" alt="">
        </a>
        <a href="#">
            <img class="carrello" src="../../../studio/svg/svg-4.svg" alt="">
        </a>
        </div>
    </div>

</template>

<script>
export default {
    name : "tariffe",
    data(){
        return{
            tariffeArr : [
                {
                    tipo      : "Basic",
                    costo     : "99",
                    concepts  :   5,
                    copyright : "Full",
                    direction : "Art",
                    creatives : "Top leven",
                    moneyback : "No"
                },
                {
                    tipo      : "Standard",
                    costo     : "119",
                    concepts  :   10,
                    copyright : "Full",
                    direction : "Art",
                    creatives : "Top leven",
                    moneyback : "No"
                },
                {
                    tipo      : "Basic",
                    costo     : "139",
                    concepts  :   15,
                    copyright : "Full",
                    direction : "Art",
                    creatives : "Top leven",
                    moneyback : "No"
                }

            ]
        }
    },
    methods : {
      scrollToTop(){
        window.scrollTo(0, 0);
      }
    }
}
</script>

<style scoped lang="scss">

@import "../../../assets/style/vars.scss";

.container-tariffe{
  width: 100%;
  background-image: url("../../../studio/img/h2-background-img-03.png");
  background-position: center;
  padding: 60px 0;
  position: relative;

  .img-tariffe{
    position: absolute;
    bottom: 33%;
    right: 0;
    display: flex;
    flex-direction: column;
    
    img{
      width: 22px;
    }

    .circle{
      background-color: $fourColor;
    }

    .carrello{
      background-color: $mainColor;
    }

    .circle, .carrello{
      padding: 6px;
      margin: 2px 0;
    }
  }

  .fa-caret-right{
  bottom: 47%;
  }

  .fa-angle-up{
    bottom: 52%
  }

  .tariffe{
    width: 65%;
    margin: 0 auto;
    display: flex;

    .standard{
      border: none;
      background-color: $tariffeBgColor;
    }

    .basic{
      border: solid 2px $tariffeBrdColor;
    }

    .basic:nth-child(2n) {   
        border: none;
        background-color: $tariffeBgColor;  
    }

    .basic:nth-child(3n) {   
        border: solid 2px $thirdColor;
    }

    .tariffa{
      width: 30%;
      margin: 2%;
      border-radius: 15px;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 35px 0 10px 0;

      .money{
        position: relative;
        font-size: 2rem;
        opacity: 1;
        padding-top: 10px;

      }
        .dollaro{
            position: absolute;
            top: 15px;
            right: -10px;
            font-size: 12px;
        }


      li{
        list-style-type: none;
        padding-top: 8px ;
        text-align: center;

      }
      button{
        margin: 25px 0 40px 0;
      }
    }

  }
}


</style>