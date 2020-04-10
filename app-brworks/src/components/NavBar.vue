<template>
  <v-app-bar app color="primary" dark>
    <div class="d-flex align-center">
      <v-btn class="shrink mr-2" href="#" text>
        <v-img
          alt="Vuetify Logo"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
        <h3>Home</h3>
      </v-btn>
    </div>
    <v-text-field
      flat
      solo-inverted
      hide-details
      prepend-inner-icon="mdi-magnify"
      label="Search"
      class="hidden-sm-and-down"
    />

    <v-btn href="#" text>
      <span class="mr-2">Login</span>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
