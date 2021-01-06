<template>
  <v-card color="basil">
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold display-3 basil--text">
        BASiL
      </h1>
    </v-card-title>

    <v-tabs
     max-width="250"
      v-model="tab"
      background-color="transparent"
      color="basil"
      grow
    >
      <v-tab
        v-for="item in items"
        :key="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item"
      >
        <v-card
          color="basil"
          flat
        >
          <v-card-text>{{ text[item] }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>
<script>
  export default {
    data () {
      return {
        tab: null,
        items: [
          'Inicio', 'Conocenos', 'Catálogos','Instalaciones','Contacto','Blog',
        ],
        text: {'Inicio':'a', 'Conocenos':'b', 'Catálogos':'c','Instalaciones':'d','Contacto':'e','Blog':'f'}  ,}
    },
  }
</script>