<template>
  <v-card>
    <v-img
      :src="require(`@/assets/backgroudporcoes.png`)"
      height="450"
      width="100%"
    >
    <v-row class="pa-10 pt-4 pb-0" justify="center">
        <v-card-title class="text-h4 mb-8 text-center w-100">
          <strong>🍟 Porções de Respeito</strong> 
        </v-card-title>
    </v-row>
    <v-row class="pa-8 pt-0">
      <v-col v-for="(item, index) in items" :key="index" cols="3" class="pt-0 pb-0">
        <v-img
          height="200"
          width="280"
          class="rounded-xl"
          :src="require(`@/assets/mais-pedidos/${item.image}`)"
        />
        <v-card-title class="text-h5 mb-8 d-flex justify-center">
          <strong>{{ item.title }}</strong>
        </v-card-title>
      </v-col>
    </v-row>
  </v-img>
  </v-card>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          { image: "imagem-09.jpg", title: "🐟 Tsunami de Sabor " },
          { image: "imagem-10.jpg", title: "Combo Big Four 💥" },
          { image: "imagem-03.jpg", title: "Fogo Jalapeño 🌶" },
          { image: "imagem-12.jpg", title: "🍤 Maré de Sabores" },
        ],
      };
    }

  }
</script>

<style>
  .transparent-card {
    background: transparent;
    box-shadow: none;
  }
</style>
