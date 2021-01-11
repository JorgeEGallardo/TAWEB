<template>
<div>
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
  <div>
    <v-app-bar
    class="bar"
    
      absolute
      dark
      shrink-on-scroll
      src=""
      style="min-width:800px;"
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(255, 255, 255,0), rgba(255, 255, 255,0)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-app-bar-title>
        <v-img class="smallSc" max-width="170" :src="img">
          </v-img>
         </v-app-bar-title>
         <div class="smallSc" style="margin-top:4rem;margin-bottom:auto;">
         <v-app-bar-title style="color:orange;margin-top:auto;font-size:1.4em; margin-bottom:auto;font-family: 'Dancing Script', cursive; margin-left:2rem">
           Tornillos Águila S.A. de C.V.
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
      <v-container class="barcontent" style="height: 130px;"></v-container>
    </v-sheet>
  </div>
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
   .bar{
     display: none;
   }
    .barcontent{
     display: none;
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
.bar{
background: rgba(248,112,47,1);
background: -moz-linear-gradient(top, rgba(248,112,47,1) 0%, rgba(241,111,92,1) 38%, rgba(240,47,23,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 100%);
background: -webkit-gradient(left top, left bottom, color-stop(0%, rgba(248,112,47,1)), color-stop(38%, rgba(241,111,92,1)), color-stop(38%, rgba(240,47,23,1)), color-stop(38%, rgba(255,255,255,1)), color-stop(38%, rgba(255,255,255,1)), color-stop(100%, rgba(255,255,255,1)));
background: -webkit-linear-gradient(top, rgba(248,112,47,1) 0%, rgba(241,111,92,1) 38%, rgba(240,47,23,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 100%);
background: -o-linear-gradient(top, rgba(248,112,47,1) 0%, rgba(241,111,92,1) 38%, rgba(240,47,23,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 100%);
background: -ms-linear-gradient(top, rgba(248,112,47,1) 0%, rgba(241,111,92,1) 38%, rgba(240,47,23,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 100%);
background: linear-gradient(to bottom, rgba(248,112,47,1) 0%, rgba(241,111,92,1) 38%, rgba(240,47,23,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 38%, rgba(255,255,255,1) 100%);
filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f8702f', endColorstr='#ffffff', GradientType=0 );
}
</style>