<template>
<div>
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="#F3752B"
      dark
      shrink-on-scroll
      src=""
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(247, 157, 92,.7), rgba(243, 117, 43,.7)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-app-bar-title>
        <v-img class="smallSc" max-width="170" :src="img">
          </v-img>
         </v-app-bar-title>
         <div class="smallSc" style="margin-top:auto;margin-bottom:auto;">
         <v-app-bar-title style="margin-top:auto;font-size:1.4em; margin-bottom:auto;font-family: 'Dancing Script', cursive; margin-left:2rem">
           Tornillos Águila <br>S.A. de C.V.
           </v-app-bar-title>
         </div>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>

     
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
      max-height="600"
    >
      <v-container style="height: 130px;"></v-container>
    </v-sheet>
  </v-card>
   <v-img class="lgSc" max-width="500" :src="imgM">
          </v-img>
</div>
</template>
<script>
export default {
  data() {
    return {
      tab: null,
      items: [
        "Inicio",
        "Conocenos",
        "Catálogos",
        "Instalaciones",
        "Contacto",
        "Blog",
      ],
      img: require("../../resources/Navbar.png"),
      imgM: require("../../resources/Mobile.png"),
      text: {
        Inicio: "a",
        Conocenos: "b",
        Catálogos: "c",
        Instalaciones: "d",
        Contacto: "e",
        Blog: "f",
      },
    };
  },
};
</script>
<style  scoped>
@media (max-width: 767px) {                  
   .smallSc {
      display: none;
   }
   .lgSc {
      display: block;
   }
}
@media (min-width: 768px) {                  
   .smallSc {
      display: block;
   }
   .lgSc {
      display: none;
   }
}
</style>