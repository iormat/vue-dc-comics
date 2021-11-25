<template>
    <div id="app">
        <Header/>

        <Main/>

        <Footer/>
    </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from "./components/Main.vue";
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
}
</script>

<style lang="scss">
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-size: 20px;
    text-transform: uppercase;
}

.container-center {
    width: 80%;
    margin: 0 auto;
}

.btn {
  background-color: transparent;
  border: 2px solid #3874D9;
  padding: 10px;
}
</style>
