<template>
  <div class="container">
    <!-- Main seuddiviso in 5 parti -->
    <div class="presentazione">
ciao
    </div>
    <div class="todo">
      <div class="container-todo-text">
        <div class="testo-todo">
          <h1>What we do?</h1>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
            Doloremque aperiam perferendis, consectetur quae rerum sit. </p>
          <button>
            <span>Read more</span>
            <i class="fa-solid fa-play"></i>
          </button>
        </div>
      </div>
      <div class="container-todo-icon">
        <div class="icone-todo">
          <div class="icona">
            <img src="../studio/img/h2-icon-01.png" alt="">
            <p>Beautifull
              <br> illustrations</p>
          </div>
          <div class="icona">
            <img src="../studio/img/h2-icon-02.png" alt=""> 
            <p>Brand
              <br> strategies</p>
          </div>       
          <div class="icona">   
            <img src="../studio/img/h2-icon-03.png" alt="">
            <p>Qualified
              <br> support</p>
          </div>   
          <div class="icona">    
            <img src="../studio/img/h2-icon-04.png" alt=""> 
            <p>Books &
              <br> magazines</p> 
          </div>      
        </div>
      </div>
      <div class="social-todo">
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

<!-- VIDEO -->

    <div class="video">
      <img src="../studio/img/main-home-video-button-img-01.png" alt="">
    </div>

<!-- TARIFFE -->

  <div class="container-tariffe">
    <div class="tariffe">
      <div class="tariffa basic">
        <h3>Basic</h3>
        <p class="money"> 99$</p>
        <ul>
          <li>
            <p>5 Design concepts</p>
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

      <div class="tariffa standard">
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
      </div>

    </div>
  </div>

<!-- DATI UTENTE -->

    <div class="datiUtente">
      <div class="container-testo-dati">
        <div class="testo-dati">
          <h1>Get in touch and say hello</h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
            <br> Possimus, beatae!.  </p>
        </div>
      </div>
      <div class="container-inserimento-dati">
        <div class="inserimento-dati">
          <div class="input-testo"><input type="text" placeholder="Comment"></div>
          <div class="input-testo name"><input type="text" placeholder="Name"></div>
          <div class="input-testo email"><input type="text" placeholder="Email"></div>
          <button>
            <span>Submit</span>
            <i class="fa-solid fa-play"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">


.todo{
  display: flex;
  height: 200px;
  margin: 60px 0;
  position: relative;

  .container-todo-text{
    width: 45%;
    position: relative;

    .testo-todo{
      width: 55%;
      position: absolute;
      right: 50px;
    }

    h1{
      font-size: 1.5rem;
    }

    p{
      font-size: 0.8rem;
      padding: 10px 0;
    }

    button{
      margin: 15px 0;
    }

  }
  .container-todo-icon{
    width: 55%;
    position: relative;

    .icone-todo{
      width: 80%;
      position: absolute;
      left: 50px;
      display: flex;
      flex-wrap: wrap;
      
      .icona{
        display: flex;
        align-items: center;
        margin: 25px 40px;
        width: 155px;

        img{
          width: 55px;
        }

        p{
          font-size: 0.9rem;
          opacity: 1;
          font-weight: bold;
          margin-left: 20px;
        }
      }
    }
  }
  .social-todo{
    display: flex;
    flex-direction: column;
  }
  .fa-caret-right{
    bottom: 50px;
  }
}



// VIDEO


.video{
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url("../studio/img/h2-img-2.jpg");
  background-size: 90%;

  height: 500px;

    img{
      width: 60px;
    }
}


// TARIFFE


.container-tariffe{
  width: 100%;
  background-image: url("../studio/img/h2-background-img-03.png");
  padding: 80px 0;

  .tariffe{
    width: 65%;
    margin: 0 auto;
    display: flex;

    .standard{
      border: none;
      background-color: #e8f3f0;
    }

    .basic{
            border: solid 1px #e9cba4;
    }

    .tariffa{
      width: 30%;
      margin: 2%;
      border-radius: 15px;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px 0 10px 0;

      .money{
        font-size: 3rem;
        opacity: 1;
        padding-top: 15px;
      }

      li{
        list-style-type: none;
        padding-top: 15px ;
        text-align: center;

        p{
          font-size: 0.8rem;
        }
      }
    }

  }
}



// DATI UTENTE


.datiUtente{
  display: flex;
  height: 200px;
  margin: 40px 0;

  .container-testo-dati{
    width: 50%;
    position: relative;

    .testo-dati{
      width: 43%;
      position: absolute;
      right: 50px;
    }

    h1{
      font-size: 2.5rem;
    }
  }
  .container-inserimento-dati{
    width: 50%;
    position: relative;

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

button{
  padding: 10px 40px;
  background-color: white;
  border: solid 1px #89aaad;
  border-radius: 20px;
  text-decoration: none;
  font-size: 0.5rem;
  margin: 40px 15px;
  cursor: pointer;

  span{
    padding-right: 5px;
  }

  .fa-play{
    height: 6px;
    padding: 1px;
  }

}


input{
  border: none;
}
.input-testo{
  border-bottom: solid 1px black;
}

</style>
