<template>
  <div>
    <!-- <div v-if="!loading"> -->
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
    <!-- </div> -->
    <!-- <loaderPage /> -->
  </div>
</template>

<script>

import presentazione from "./commons/Main/presentazione.vue";
import progetti from "./commons/Main/progetti.vue";
import todo from "./commons/Main/todo.vue";
import videoProject  from "./commons/Main/videoProject .vue";
import tariffe from "./commons/Main/tariffe.vue";  
import datiUtente from "./commons/Main/datiUtente.vue";
// import loaderPage from "./select/loaderPage.vue"



export default {
  name: 'Main',
  components : {
    presentazione,
    progetti,
    todo,
    videoProject,
    tariffe,
    datiUtente,
    // loaderPage
  },
  // data(){
  //   return{
  //     loading : false
  //   }
  // },
  // created() {
  //   this.loading = true  
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container{
  width: 100%;
  height: 100%;
}

</style>
