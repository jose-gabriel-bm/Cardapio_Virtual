<template>
  <v-app>
    <menu-superior/>

    <v-main>
      <index-pagina/>
    </v-main>
    <redirecionar-whatsapp/>
       
    <rodape-cardapio/>
  </v-app>
</template>

<script>
import indexPagina from '@/views/indexPagina.vue';
import menuSuperior from '@/components/menus/menuSuperior.vue';
import rodapeCardapio from '@/components/menus/rodapeCardapio.vue';
import redirecionarWhatsapp from '@/components/menus/redirecionarWhatsapp.vue';

export default {
  name: 'App',

  components: {
    indexPagina,
    menuSuperior,
    rodapeCardapio,
    redirecionarWhatsapp
  },

  data: () => ({
    //
  }),
};
</script>
<style>
html, body {
  overflow-y: auto;
  scrollbar-width: none; /* Para Firefox */
}

html::-webkit-scrollbar {
  display: none; /* Para Chrome, Safari e Edge */
}

</style>
