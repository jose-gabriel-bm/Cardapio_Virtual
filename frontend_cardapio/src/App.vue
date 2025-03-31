<template>
  <v-app>
    <menu-superior/>

    <v-main>
      <HelloWorld/>
    </v-main>
    
    <rodape-cardapio/>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import MenuSuperior from '@/components/menus/menuSuperior.vue';
import rodapeCardapio from '@/components/menus/rodapeCardapio.vue';

export default {
  name: 'App',

  components: {
    HelloWorld,
    MenuSuperior,
    rodapeCardapio
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
