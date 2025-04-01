<template>
  <v-div>
    <carrosel-inicial/>

  </v-div>
</template>
  
<script>
  import carroselInicial from '@/components/geral/carroselInicial.vue';
  
  export default {
    name: 'IndexPagina',
  
    components: {
      carroselInicial
    },
  
    data: () => ({
      //
    }),
  };
</script>

  