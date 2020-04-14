<template>
  <v-card v-repeat="jobInfo" >
    <v-card-title>
        {{ title }}
    </v-card-title>
    <v-card-subtitle>
        {{ price }}
    </v-card-subtitle>

    <v-card-actions>
      <v-btn icon @click="show = !show">
        <v-icon>{{ show ? 'mdi-chevron-up-circle-outline' : 'mdi-chevron-down-circle-outline' }}</v-icon>
      </v-btn>
    </v-card-actions>

     <v-expand-transition>
      <div v-show="show">        
        <v-divider/>
        <v-card-text>
          {{ textInfo }}
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>


<script>

export default {
        name: 'Card',
          props: {
            title: String,
            price: String,
            textInfo: String,

          },
          data: () => ({
            show: false,

        }),

        components: {
           
        },

}
</script>

<style>

</style>