<template>
    <div style="min-height:100vh;">
  <Navbar></Navbar>
  <v-row>
      <v-col cols="12" md=6>
          <v-img :src="img"></v-img>
      </v-col>
      <v-col cols="12" md=6>
          <div style="text-align:center">
              <div class="titleM">Misión</div>
              <div class="contentM">Es ser una empresa líder en el negocio de herramientas, tornillos y accesorios satisfaciendo las necesidades de nuestros clientes con productos de óptima calidad y respaldos con un excelente servicio.</div><br>
              <div class="titleM">Visión</div>
              <div class="contentM">Ser una empresa reconocida a nivel regional por su amplio surtido y disponibilidad en todo tipo de tornillería y herramienta, mejorando continuamente nuestros estándares de calidad y valor agregado en la distribución de nuestros productos, dándole al cliente más alternativas, mejorando nuestra atención y servicio.</div>
          </div>
      </v-col>
  </v-row>
    </div>
</template>
<script>
export default {
    data(){
        return{
            img:require("../../resources/aguila.png"),
        }
    }
}
</script>
<style scoped>
.titleM{
    color: #f8702f;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 1.5rem;
    margin:1rem;
}
.contentM{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 1.2rem;
    font-style: italic;
}
</style>