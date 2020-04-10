<template>
  <v-app>
    <NavBar />
    <v-content>
      <MainBlock />
    </v-content>
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import MainBlock from "./components/MainBlock.vue";

export default {
  name: "App",

  components: {
    NavBar,
    MainBlock
  },

  data: () => ({
    //
  })
};
</script>
<style lang="scss">
@import "./styles/main.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
