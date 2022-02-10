<template>
      <div class="container">
<!-- Main suddiviso in 6 parti -->

  <!-- PRESENTAZIONE -->

        <presentazione />

  <!-- PROGETTI -->

        <progetti />

  <!-- TODO -->

        <todo />

  <!-- VIDEO -->

        <videoProject />

  <!-- TARIFFE -->

        <tariffe />

  <!-- DATI UTENTE -->

        <datiUtente />

      </div>
</template>

<script>

import presentazione from "./commons/Main/presentazione.vue";
import progetti from "./commons/Main/progetti.vue";
import todo from "./commons/Main/todo.vue";
import videoProject  from "./commons/Main/videoProject .vue";
import tariffe from "./commons/Main/tariffe.vue";  
import datiUtente from "./commons/Main/datiUtente.vue";



export default {
  name: 'Main',
  components : {
    presentazione,
    progetti,
    todo,
    videoProject,
    tariffe,
    datiUtente
  },
  data(){
    return{
      loading : true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container{
  width: 100%;
  height: 100%;
}


// .progetti{
//   height: 1082px;
//   background-image: url("../studio/img/h2-background-img-02 (1).png");
//   background-repeat: repeat;
//   background-size: 85%;
//   background-position: 6px;
//   position: relative;

//   .fa-caret-right{
//     bottom: 16%;
//   }

//   .fa-angle-up{
//     bottom: 18.5%
//   }


//   .jumbo-progetti{
//     display: flex;
//     flex-wrap: wrap;
//     width: 720px;
//     margin: -90px auto;

//     .progetto{
//       height: 360px;
//       img{
//         width: 360px;
//       }
//     }
//   }
// }

// PRESENTAZIONE


// .presentazione{
//   display: flex;
//   justify-content: center;
//   align-items: center;
//   height: 361px;
//   width: 100%;
//   margin: 0 0 30px 0;
//   background-image: url("../studio/img/h2-background-img-02.png");
//   background-repeat: repeat;
//   background-size: 85%;
//   position: relative;

//   .fa-caret-right{
//     bottom: -130%
//   }

//   .fa-angle-up{
//     bottom: -122.5%
//   }

//   .jumbo-presentazione{
//   display: flex;
//   align-items: center;
//   width: 70%;
//   margin: 0 auto;
//   }

//   .container-titolo{
//     width: 75%;

//     .titolo-presentazione{
//       width: 90%;
      
//       h1{
//         font-size: 1.9rem;
//         line-height: 1.1;
//       }
//     }
//   }
//   .container-desctizione{
//     width: 90%;

//     .descrizione-presentazione{
//       width: 95%;
//     }
//     p{
//       padding: 10px 0;
//     }
//   }
// }


// todo 

// .todo{
//     position: relative;

//   .container-todo{
//     display: flex;
//     height: 200px;
//     margin: 60px auto;
//     width: 85%;

//     .fa-caret-right{
//         bottom: 50px;
//       }
      
//     .fa-angle-up{
//       bottom: 77px;
//     }

//     .container-todo-text{
//       width: 42%;
//       position: relative;

//       .testo-todo{
//         width: 55%;
//         position: absolute;
//         right: 25px;
//       }

//       h1{
//         font-size: 1.5rem;
//       }

//       p{
//         padding: 10px 0;
//       }

//       button{
//         margin: 15px 0;
//       }

//     }
//     .container-todo-icon{
//       width: 55%;
//       position: relative;

//       .icone-todo{
//         width: 80%;
//         position: absolute;
//         display: flex;
//         flex-wrap: wrap;
        
//         .icona{
//           display: flex;
//           align-items: center;
//           margin: 25px 40px;
//           width: 155px;

//           img{
//             width: 55px;
//           }

//           p{
//             opacity: 1;
//             font-weight: bold;
//             margin-left: 20px;
//           }
//         }
//       }
//     }
//     .social-todo{
//       display: flex;
//       flex-direction: column;
//       position: absolute;
//       right: 20px;
//       bottom: 55%;

//       a{
//         .fa-facebook-f, .fa-instagram, .fa-twitter , .fa-pinterest-p{
//           width: 8px;
//           color: black;
//         }
//       }    
//     }
//   }
// }

// VIDEO


// .video{
//   display: flex;
//   justify-content: center;
//   align-items: center;
//   background-image: url("../studio/img/h2-img-2.jpg");
//   background-size: 85%;
//   background-position:center;
//   height: 350px;
//   position: relative;

//   .fa-caret-right{
//     bottom: 45%;
//   }

//   .fa-angle-up{
//       bottom: 52.5%
//     }

//   img{
//     width: 60px;
//   }
// }


// TARIFFE


// .container-tariffe{
//   width: 100%;
//   background-image: url("../studio/img/h2-background-img-03.png");
//   background-position: center;
//   padding: 60px 0;
//   position: relative;

//   .img-tariffe{
//     position: absolute;
//     bottom: 33%;
//     right: 0;
//     display: flex;
//     flex-direction: column;
    
//     img{
//       width: 22px;
//     }

//     .circle{
//       background-color: red;
//     }

//     .carrello{
//       background-color: white;
//     }

//     .circle, .carrello{
//       padding: 6px;
//       margin: 2px 0;
//     }
//   }

//   .fa-caret-right{
//   bottom: 47%;
//   }

//   .fa-angle-up{
//     bottom: 52%
//   }

//   .tariffe{
//     width: 65%;
//     margin: 0 auto;
//     display: flex;

//     .standard{
//       border: none;
//       background-color: #e8f3f0;
//     }

//     .basic{
//       border: solid 1px #e9cba4;
//     }

//     .tariffa{
//       width: 30%;
//       margin: 2%;
//       border-radius: 15px;
//       display: flex;
//       flex-direction: column;
//       align-items: center;
//       padding: 35px 0 10px 0;

//       .money{
//         font-size: 2rem;
//         opacity: 1;
//         padding-top: 10px;
//       }

//       li{
//         list-style-type: none;
//         padding-top: 8px ;
//         text-align: center;

//       }
//       button{
//         margin: 25px 0 40px 0;
//       }
//     }

//   }
// }


// DATI UTENTE


// .datiUtente{
//   display: flex;
//   height: 160px;
//   margin: 80px 0;
//   position: relative;

//   .fa-caret-right{
//     bottom: 85%;
//   }

//   .fa-angle-up{
//     bottom: 101%;
//   }

//   .container-testo-dati{
//     width: 50%;
//     position: relative;

//     .testo-dati{
//       width: 43%;
//       position: absolute;
//       right: 50px;
//     }

//     h1{
//       font-size: 2.3rem;
//       line-height: 1.1;
//     }

//     p{
//       margin: 10px 0;
//       width: 300px;
//     }
//   }
//   .container-inserimento-dati{
//     width: 50%;
//     position: relative;
//     margin: -40px 0;

//     .inserimento-dati{
//       width: 398px;
//       position: absolute;
//       left: 50px;
//     }
    
//     .input-testo{
//       margin: 40px 0 0 15px;
//     }

//     .name,.email{
//       display: inline-block;
//     }
//   }
// }

// button{
//   padding: 10px 40px;
//   background-color: white;
//   border: solid 1px #89aaad;
//   border-radius: 20px;
//   text-decoration: none;
//   font-size: 0.5rem;
//   margin: 40px 15px;
//   cursor: pointer;

//   span{
//     padding-right: 5px;
//   }

//   .fa-play{
//     height: 6px;
//     padding: 1px;
//   }
//   .fa-caret-right{
//   bottom: 85%;
//   }
// }

// input{
//   border: none;
// }
// .input-testo{
//   border-bottom: solid 1px black;
// }

</style>
