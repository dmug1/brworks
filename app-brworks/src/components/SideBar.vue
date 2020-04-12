<template>
  <div id="SideBar">
    <v-card color=" lighten-2">
      <v-card-title class="headline lighten-3">
        Filtros
      </v-card-title>

      <v-card-text>
        <v-autocomplete
          v-model="cidade"
          :items="items"
          :loading="isLoading"
          color="white"
          hide-no-data
          hide-selected
          item-text="Description"
          label="Cidade"
          placeholder="Digite a cidade"
          return-object
        ></v-autocomplete>
      </v-card-text>
      <v-divider></v-divider>
      <v-card-text>
        <v-autocomplete
          v-model="servico"
          :items="services"
          :loading="isLoading"
          color="white"
          hide-no-data
          hide-selected
          item-text="Description"
          label="Serviço"
          placeholder="Digite o serviço"
          return-object
        ></v-autocomplete>
      </v-card-text>

      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn
          :disabled="!cidade"
          color="grey darken-3"
          @click="(cidade = null), (servico = null)"
        >
          Limpar
          <v-icon right>mdi-close-circle</v-icon>
        </v-btn>
      </v-card-actions>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    descriptionLimit: 60,
    items: ["Brisbane", "Sydney"],
    services: ["Salao de Beleza", "Mecanico", "Carreto", "Transfer", "Comida"],
    isLoading: false,
    cidade: null,
    servico: null,
    search: null
  })
};
</script>

<style></style>
