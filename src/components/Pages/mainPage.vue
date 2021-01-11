<template>
  <div style="min-height:100vh;">
  <Navbar></Navbar>
  <div style="max-width:1200px; margin-right:auto;margin-left:auto;color:orange">
   <v-tabs
    v-model="tab"
    fixed-tabs
    center-active
    background-color="#ffffa"
    style="color:black"
  >
    <v-tab>
      <b>Inicio</b>
    </v-tab>
    <v-tab>
      <b>Conócenos</b>
    </v-tab>
    <v-tab>
      <b>Catálogos</b>
    </v-tab>
    <v-tab>
      <b>Instalaciones</b>
    </v-tab>
    <v-tab>
      <b>Contacto</b>
    </v-tab>
  </v-tabs>
   </div>
   <div  id="divCont">
   <v-tabs-items  v-model="tab">
      <v-tab-item
       
      >
      
        <Inicio></Inicio>
     
      </v-tab-item>
       <v-tab-item
       
      >
        <v-card flat>
          <v-card-text><Contactanos></Contactanos></v-card-text>
        </v-card>
      </v-tab-item>
       <v-tab-item
       
      >
        <v-card flat>
          <v-card-text><Catalogos></Catalogos></v-card-text>
        </v-card>
      </v-tab-item>
       <v-tab-item
       
      >
        <v-card flat>
          <v-card-text><Instalaciones></Instalaciones></v-card-text>
        </v-card>
      </v-tab-item>
       <v-tab-item
       
      >
        <v-card flat>
          <v-card-text><Contacto></Contacto></v-card-text>
        </v-card>
      </v-tab-item>

    </v-tabs-items>
   </div>
  <Footer> </Footer>
  </div>
</template>

<script>
import Navbar from "../Bars/Navbar.vue"
import Footer from "../Bars/footer.vue"
import Instalaciones from "./InstalacionesPage.vue"
import Inicio from "./InicioPage.vue"
import Catalogos from "./CatalogosPage.vue"
import Contactanos from "./ContactanosPage.vue"
import Contacto from "./ContactoPage.vue"
export default {
    components:{
        Navbar, 
        Footer,
        Instalaciones,
        Inicio,
        Catalogos,
        Contactanos,
        Contacto
    },
     data () {
      return {
        tab: null,
      }
      }
}
</script>

<style>
@media (max-width: 1200px) {                  
   #divCont {
      margin-right: 0rem;
      margin-left: 0rem;
   }
   
}
@media (min-width: 1900px) {                  
   #divCont {
      margin-right: 10%;
      margin-left: 10%;
   }
}
@media (min-width: 1201px ) and (max-width: 1899px) {                  
   #divCont {
      margin-right: 5%;
      margin-left: 5%;
   }
}
b{
  font-size:1.2rem
}
</style>