<template>
  <v-app>
    <Navbar></Navbar>
    <Carousel></Carousel>
  </v-app>
</template>

<script>
import Navbar from "./Bars/navbar.vue";
import Carousel from "./Components/Carousel.vue";
export default {
  components: { Navbar, Carousel },
  data() {
    return {};
  },
};
</script>

<style>
</style>>