<template>
  <div id="app" class="md-app">
    <link
      rel="stylesheet"
      href="//fonts.googleapis.com/css?family=Roboto:400,500,700,400italic|Material+Icons"
    >
    <Header gameName="Titan" class="md-app-toolbar" md-mode="fixed"/>
    <Main class="md-app-content"/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import VueMaterial from "vue-material";
import "vue-material/dist/vue-material.min.css";
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

Vue.use(VueMaterial);

@Component({
  components: {
    Header,
    Main
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
</style>
