<template>
  <v-container fluid>
    <v-row dense>
      <v-col v-for="job in jobInfo" :key="job.id" :cols="4">
        <card
          :title="job.title"
          :price="job.price"
          :textInfo="job.textInfo"
          :src="job.src"
          :rating="job.rating"
        />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Card from "./Card.vue";

export default {
  name: "contentblock",
  data: () => ({
    jobInfo: [
      {
        id: 1,
        title: "Cozinhar bolo top",
        price: "$19,90",
        textInfo: " Fazer um bolo",
        src: "https://cdn.vuetifyjs.com/images/cards/docks.jpg",
        rating: 4.5
      },
      {
        id: 2,
        title: "Jardineiro",
        price: "$189,90",
        textInfo: " Cortar a grama",
        src: "https://cdn.vuetifyjs.com/images/cards/docks.jpg",
        rating: 4
      },
      {
        id: 3,
        title: "Mecanico",
        price: "$99,90",
        textInfo: " Lixar a tinta",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        rating: 3.5
      },
      {
        id: 4,
        title: "Concertar pc",
        price: "$19,90",
        textInfo: " Fazer um bolo",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        rating: 5
      },
      {
        id: 5,
        title: "Prepar orçamento",
        price: "$189,90",
        textInfo: " Cortar a grama",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        rating: 3
      },
      {
        id: 6,
        title: "Limpar a vala",
        price: "$99,90",
        textInfo: " Lixar a tinta",
        src: "",
        rating: 4.5
      }
    ]
  }),

  components: {
    Card
  }
};
</script>

<style>
</style>


