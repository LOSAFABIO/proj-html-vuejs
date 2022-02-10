<template>
<div>
  <!-- <div v-if="!loading" id="app"> -->
    <Header />
    <Main />
    <Footer />
  <!-- </div> -->
  <!-- <loader v-else /> -->
</div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
// import loader from "./components/select/loader.vue"
// import axios from "axios"



export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    // loader
  },
    // created() {
    //   this.getLoading();
    // },
    // methods:{
    //     getLoading(){
    //         axios.get(this.apiURL)
    //         .then(() => {
    //             // handle success
    //             this.loading = false
    //         })
    //         .catch(function (error) {
    //             // handle error
    //             console.log(error);
    //         })
    //     }
    // }
}
</script>

<style lang="scss">

@import "assets/style/Globals.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
} 
</style>
