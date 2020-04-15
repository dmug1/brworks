<template>
  <v-app>
    <NavBar />
    <SideBar />
    <v-content>
      <ContentBlock />
    </v-content>
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import SideBar from "./components/SideBar.vue";
import ContentBlock from "./components/ContentBlock.vue";

export default {
  name: "App",

  components: {
    NavBar,
    SideBar,
    ContentBlock
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
