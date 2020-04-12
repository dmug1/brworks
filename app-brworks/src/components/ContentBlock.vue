<template>
  <v-container id="ContentBlock">
    <v-layout row>
      <v-flex xs12 md4> 
       <card class="cardStyle"/>
      </v-flex>
      <v-flex xs12 md4> 
       <card class="cardStyle"/>
      </v-flex>
      <v-flex xs12 md4> 
       <card class="cardStyle"/>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Card from './Card.vue'

export default {
        name: 'contentblock',
        components: {
            Card
        },

}
</script>

<style>

</style>


