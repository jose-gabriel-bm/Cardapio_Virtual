<template>
  <div>
    <v-row class="pa-10 pt-0 pb-0" justify="center">
      <v-card elevation="0" class="transparent-card">
        <v-card-title class="text-h4 mb-8 text-center w-100">
          <strong>🔥 Os Favoritos da Casa!</strong> 
        </v-card-title>
      </v-card>
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

  </div>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          { image: "imagem-01.jpg", title: "Supremo Smash 🍔" },
          { image: "imagem-02.png", title: "Croc Frango Gold 🐔" },
          { image: "imagem-03.jpg", title: "Fogo Jalapeño 🌶" },
          { image: "imagem-04.jpg", title: "Cheddar Avalanche 🧀" },
          { image: "imagem-05.jpg", title: "Fumaça & Brasa 🔥" },
          { image: "imagem-06.jpg", title: "Rei Barbecue 👑" },
          { image: "imagem-07.png", title: "Taco Prime ✨" },
          { image: "imagem-08.jpg", title: "Pack Delícia 🍟 " },
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
