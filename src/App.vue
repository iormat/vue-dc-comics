<template>
    <div id="app">
        <AppHeader/>

        <AppMain/>

        <AppFooter/>
    </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from "./components/AppMain.vue";
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
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
  padding: 10px 15px;
  border: 2px solid #3874D9;
}
</style>
