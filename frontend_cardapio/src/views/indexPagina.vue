<template>
  <v-div>
    <carrosel-inicial/>
    <sobre-empresa/>
    <receitas-favoritas/>
    <todas-porcoes/>
    <geral-bebidas/>
    <!-- <geral-sobremesa/> -->
  </v-div>
</template>
  
<script>
  import carroselInicial from '@/components/geral/carroselInicial.vue';
  import sobreEmpresa from '@/components/geral/sobreEmpresa.vue';
  import receitasFavoritas from '@/components/geral/receitasFavoritas.vue';
  import todasPorcoes from '@/components/geral/todasPorcoes.vue';
  import geralBebidas from '@/components/geral/geralBebidas.vue';
  // import geralSobremesa from '@/components/geral/geralSobremesa.vue';

  export default {
    name: 'IndexPagina',
  
    components: {
      carroselInicial,
      sobreEmpresa,
      receitasFavoritas,
      todasPorcoes,
      // geralSobremesa,
      geralBebidas
    },
  
    data: () => ({
      //
    }),
  };
</script>

  