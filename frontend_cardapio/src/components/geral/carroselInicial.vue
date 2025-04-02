<template>
  <v-carousel
    cycle
    hide-delimiter-background
    :show-arrows="false"
    touchless
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: require('@/assets/carrosel-01.png'),
          },
          {
            src: require('@/assets/carrosel-02.png'),
          },
          {
            src: require('@/assets/carrosel-03.png'),
          },
        ],
      }
    },
  }
</script>

<style>
  .v-carousel {
    scroll-behavior: auto !important;
    overflow: hidden !important;
  }
</style>