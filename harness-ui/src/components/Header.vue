<template>
  <div class="header">
    <md-toolbar>
      <div class="md-toolbar-row">
        <h1 class="md-title">{{ gameName }}</h1>
      </div>
      <div class="md-toolbar-row">
        <md-menu>
          <md-button @click="parent.showLaunch = true">Launch</md-button>
        </md-menu>
        <md-menu>
          <md-button>Host Actions</md-button>
        </md-menu>
        <md-menu>
          <md-button>Client Messaging</md-button>
        </md-menu>
      </div>
    </md-toolbar>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Header extends Vue {
  @Prop() private gameName!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
