<template>
  <v-container id="ContentBlock">
    <card />
    <card />    
    <card />
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


