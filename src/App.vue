<template>
    <div id="app">
        <Header/>

        <Footer/>
    </div>
</template>

<script>
import Header from './components/Header.vue';

import Footer from './components/Header.vue';


export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
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
}
.container-center {
    width: 80%;
    margin: 0 auto;
}
</style>
