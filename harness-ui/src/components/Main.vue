<template>
  <div class="main">
    <md-drawer :md-active.sync="parent.showLaunch">
      <md-button>Launch</md-button>
    </md-drawer>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Main extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
