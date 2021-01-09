<template>
  <div id="Inicio">
    <v-row>
      <v-col cols="12" md="8"><Gallery></Gallery></v-col>

      <v-col cols="12" md="4">
        <v-img :src="imgs[0]"> </v-img>
        <div>
          <h1>Acceso a Plataforma</h1>
          <br />
          <v-btn
          @click="redirect(0)"
            block
            elevation="9"
            rounded
            x-large
            dark
            color="#ff7b54"
            style="height: 75px"
            ><h3>Tornillos Águila</h3></v-btn
          >
          <br />
          <v-btn
           @click="redirect(1)"
            block
            elevation="9"
            rounded
            x-large
            dark
            color="#65d6ce"
            style="height: 75px"
            ><h3>Águila Proveedora</h3></v-btn
          >
        </div>
      </v-col>
    </v-row>
    <v-row style="color: orange">
      <v-col style="padding: 3%" cols="12" md="3">
        <h1 style="background-color: #ff7b54; font-size: 2rem; color: white;height:3rem">
          Truper
        </h1>
        <v-img :src="imgs[1]"></v-img>
      </v-col>
       <v-col style="padding: 3%" cols="12" md="3">
        <h1 style="background-color: #ff7b54; font-size: 2rem; color: white;height:3rem">
          Evans
        </h1>
        <v-img :src="imgs[2]"></v-img>
      </v-col>
       <v-col style="padding: 3%" cols="12" md="3">
        <h1 style="background-color: #ff7b54; font-size: 2rem; color: white;height:3rem">
          Fischer
        </h1>
        <v-img :src="imgs[3]"></v-img>
      </v-col>
       <v-col style="padding: 3%" cols="12" md="3">
        <h1 style="background-color: #ff7b54; font-size: 2rem; color: white;height:3rem">
          Nuestras marcas
        </h1>
        <v-img :src="imgs[4]"></v-img>
      </v-col>
    </v-row>
  </div>
</template>
<script>
import Gallery from "../components/Carousel.vue";
export default {
  components: {
    Gallery,
  },
  data() {
    return {
      imgs: [
        require("../../resources/Distribuidor.jpg"),
        require("../../resources/Motor2.jpg"),
        require("../../resources/Motor.jpg"),
        require("../../resources/Fischer.jpg"),
        require("../../resources/Conoce.jpg"),
      ],
    };
  },methods:{
       redirect(suc) {
           if(suc==0)
          window.location.href = "http://aguiladgo.dyndns.org:1945/B2B/index.php"
          if(suc==1)
          window.location.href = "http://aguiladgo.dyndns.org:1945/B2BAP/index.php"
      },
  },
};
</script>

<style>
</style>
