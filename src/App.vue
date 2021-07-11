<template>
  <div id="app">
    <header-component></header-component>
    <body-component></body-component>
    <footer-compoent></footer-compoent>
  </div>
</template>

<script>
import headerComponent from "./components/headerComponent.vue";
import bodyComponent from "./components/bodyComponent.vue";
import footerCompoent from "./components/footerComponent.vue";

export default {
  name: "App",
  components: {
    headerComponent,
    bodyComponent,
    footerCompoent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
