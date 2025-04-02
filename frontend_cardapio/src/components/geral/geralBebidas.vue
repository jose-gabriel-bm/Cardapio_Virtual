<template>
  <v-row class="pa-10">
    <v-col cols="7" class="pa-10 d-flex flex-column align-center" >
      <v-card-title class="text-h4 mb-8 d-flex justify-center">
        <strong>Bebidas</strong> 
      </v-card-title>
      <v-img
        height="280"
        width="480"
        class="rounded-xl"
        :src="require('@/assets/backgroudBebidas.png')"
      />
    </v-col>
    <v-col cols="5" class="pa-10">
      <v-card elevation="0">
        <v-row v-for="drink in drinks" :key="drink.name">
          <v-col cols="4">
            <v-img
              height="40"
              width="60"
              :src="require(`@/assets/${drink.image}`)"
            />
          </v-col>
          <v-col cols="5" class="d-flex justify-center">
            <v-card-subtitle style="text-align: left !important; font-size: 15px;">
              {{ drink.name }}
            </v-card-subtitle>
          </v-col>
          <v-col cols="3" class="d-flex justify-center">
            <v-card-subtitle style="text-align: left !important; font-size: 15px;">
              {{ drink.price }}
            </v-card-subtitle>
          </v-col>
        </v-row>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
  export default {
    data() {
      return {
        drinks: [
          { name: 'Caipirinha Suprema', price: 'R$ 15,00', image: 'drinks/caipirinha.png' },
          { name: 'Mojito Fresh', price: 'R$ 18,00', image: 'drinks/mojito.png' },
          { name: 'Piña Tropical', price: 'R$ 22,00', image: 'drinks/pina.png' },
          { name: 'Sucos', price: 'R$ 11,00', image: 'drinks/suco.png' },
          { name: 'Soda Tropical', price: 'R$ 23,50', image: 'drinks/soda.png' },
          { name: 'Shope', price: 'R$ 12,00', image: 'drinks/shope.png' },
        ]
      };
    }
  };
</script>

<style>
  .transparent-card {
    background: transparent;
    box-shadow: none;
  }
</style>