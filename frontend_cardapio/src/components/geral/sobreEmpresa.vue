<template>
  <v-row class="pa-10">
    <v-col cols="6" class="pa-10">
      <v-img
        height="400"
        width="480"
        class="rounded-xl"
        :src="require('@/assets/imagemSobre.png')"
      />
    </v-col>
    <v-col cols="6">
      <v-card elevation="0">
        <v-card-title class="text-h5 mb-8 d-flex justify-center">
          <strong>O Sabor Que Conta Nossa História</strong> 
        </v-card-title>

        <v-card-subtitle class="text-h6">
          Nossa paixão por hambúrgueres começou com o desejo de criar algo único.
          Aqui, cada ingrediente é escolhido com cuidado, cada receita é testada com dedicação 
          e cada hambúrguer é preparado para proporcionar uma experiência inesquecível.
        </v-card-subtitle>

        <v-card-subtitle class="text-h6 pt-0">
          Acreditamos que um bom hambúrguer vai além do pão e da carne 
          é uma combinação perfeita de ingredientes frescos, técnica artesanal 
          e muito amor pelo que fazemos.
        </v-card-subtitle>

        <v-card-actions class="d-flex justify-center align-center"> 
          <v-btn
            class="ml-2 mt-0 pa-6"
            rounded
            large
            color="#ffb301"
          >
            SAIBA MAIS
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<style>
  .transparent-card {
    background: transparent;
    box-shadow: none;
  }
</style>