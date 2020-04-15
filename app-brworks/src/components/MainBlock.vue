<template>
  <div id="MainBlock" class="row">
    <ContentBlock class="col-3-of-4" />
  </div>
</template>

<script>
import ContentBlock from "./ContentBlock.vue";

export default {
  name: "mainblock",
  components: {
    ContentBlock
  }
};
</script>

<style>
</style>
