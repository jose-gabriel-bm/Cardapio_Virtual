<template>
  <v-app-bar
    app
    dark
    color="black"
  >
    <div class="d-flex align-center">
      <v-img
        alt="Vuetify Logo"
        class="shrink mr-2"
        contain
        src="@/assets/logo.png"
        transition="scale-transition"
        width="25"
      />
    </div>
    <v-spacer></v-spacer>
    <div class="d-flex align-center ml-8">
      <v-btn text to="/">Início</v-btn>
      <v-btn text to="/produtos">Produtos</v-btn>
      <v-btn text to="/sobre">Sobre</v-btn>
    </div>
    <v-spacer></v-spacer>
    <v-btn
      color="accent-4"
      icon
      class="pa-0"
    >
      <v-icon color="#ffb301">mdi-whatsapp</v-icon>
    </v-btn>
    <v-btn
      class="pa-0"
      color="accent-4"
      icon
    >
      <v-icon color="#ffb301">mdi-cart-variant</v-icon>
    </v-btn>
  </v-app-bar>
</template>

