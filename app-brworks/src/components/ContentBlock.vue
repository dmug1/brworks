<template>
  <v-container id="ContentBlock">
    <v-layout row>
      <v-flex v-for="job in jobInfo" :key="job.id" xs12 md4 class="cardHolder"> 
       <card class="cardStyle" 
        :title="job.title"
        :price="job.price"
        :textInfo="job.textInfo"
        />
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Card from './Card.vue'

export default {
        name: 'contentblock',
          data: () => ({
            jobInfo: [
              {id:1, title:'Cozinheiro',price:'$19,90', textInfo:' Fazer um bolo'},
              {id:2, title:'Jardineiro',price:'$189,90', textInfo:' Cortar a grama'},
              {id:3, title:'Mecanico',price:'$99,90', textInfo:' Lixar a tinta'},
            ]
        }),    
        components: {
            Card
        },

}
</script>

<style>

</style>


