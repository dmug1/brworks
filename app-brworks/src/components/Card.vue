<template>
  <v-card v-repeat="jobInfo" class="mx-auto my-12">
    <v-img
      :src="src"
      class="white--text align-end"
      gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
      height="200px"
    >
      <v-icon>mdi-image</v-icon>
      <v-card-title>{{title}}</v-card-title>
    </v-img>
    <v-card-text>
      <v-row align="center" class="mx-0" background-color="white">
        <v-rating :value="rating" color="amber" dense half-increments readonly size="14"></v-rating>

        <div class="grey--text ml-4">{{rating}}</div>
      </v-row>
    </v-card-text>
    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn icon @click="show = !show">
        <v-icon>{{ show ? 'mdi-chevron-up-circle-outline' : 'mdi-chevron-down-circle-outline' }}</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-bookmark</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-share-variant</v-icon>
      </v-btn>
    </v-card-actions>
    <v-expand-transition>
      <div v-show="show">
        <v-divider />

        <v-card-text>
          <div class="my-4 subtitle-1">{{ price }}/hr</div>

          <div class="my-4 subtitle-1">{{ textInfo }}</div>
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>


<script>
export default {
  name: "Card",
  props: {
    title: String,
    price: String,
    textInfo: String,
    src: String,
    rating: Number
  },
  data: () => ({
    show: false
  }),

  components: {}
};
</script>

<style>
</style>