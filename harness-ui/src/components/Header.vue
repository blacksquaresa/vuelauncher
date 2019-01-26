<template>
  <div class="header">
    <h1>{{ gameName }}</h1>
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
.header {
  margin: 0px;
  padding: 0px;
  position: absolute;
  top: 0px;
  left: 0px;
  right: 0px;
  height: 99px;
  border-bottom: solid 1px #ccc;
}
</style>
