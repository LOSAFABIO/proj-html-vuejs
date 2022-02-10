<template>
    <div class="todo">
        <div class="container-todo">
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
                    <div v-for="(elemento, indice) in todoArr" :key="indice" class="icona">
                        <img :src="elemento.image" alt="">
                        <p>{{elemento.testo}}</p>
                    </div>
                </div>
            </div>
            <div class="social-todo">
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
    name : "todo",
    data(){
        return{
            todoArr : [
                {
                    image : require("../../../studio/img/h2-icon-01.png"),
                    testo  : "Beautifull illustrations"
                },
                {
                    image : require("../../../studio/img/h2-icon-02.png"),
                    testo  : "Beautifull illustrations"
                },
                {
                    image : require("../../../studio/img/h2-icon-03.png"),
                    testo  : "Beautifull illustrations"
                },
                {
                    image : require("../../../studio/img/h2-icon-04.png"),
                    testo  : "Books & magazines"
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">

.todo{
    position: relative;

  .container-todo{
    display: flex;
    height: 200px;
    margin: 60px auto;
    width: 85%;

    .fa-caret-right{
        bottom: 50px;
      }
      
    .fa-angle-up{
      bottom: 77px;
    }

    .container-todo-text{
      width: 42%;
      position: relative;

      .testo-todo{
        width: 55%;
        position: absolute;
        right: 25px;
      }

      h1{
        font-size: 1.5rem;
      }

      p{
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
      position: absolute;
      right: 20px;
      bottom: 55%;

      a{
        .fa-facebook-f, .fa-instagram, .fa-twitter , .fa-pinterest-p{
          width: 8px;
          color: black;
        }
      }    
    }
  }
}


</style>