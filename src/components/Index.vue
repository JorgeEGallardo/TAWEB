<template>
  <v-app>
 <Navbar></Navbar>
    <v-btn color="success">Si ves un botón que no sea blanco funciono bien</v-btn>
  </v-app>
</template>

<script>
import Navbar from './Bars/navbar.vue';
export default {
  components: {Navbar},
  data() {
    return {
    };
  },
};
</script>

<style>
</style>>