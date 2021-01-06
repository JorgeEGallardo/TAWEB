<template>
  <v-app>
 <Navbar></Navbar>
    <v-btn color="success">Si ves un botón que no sea blanco funciono bien</v-btn>
sss
 <Carousel></Carousel>
 ssss
  </v-app>
</template>

<script>
import Navbar from './Bars/navbar.vue';
import Carousel from './Components/Carousel.vue';
export default {
  components: {Navbar, Carousel},
  data() {
    return {
    };
  },
};
</script>

<style>
</style>>