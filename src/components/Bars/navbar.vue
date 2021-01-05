<template>
<v-card>
  <v-toolbar
      color="white"
      flat
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Page title</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>

      <template v-slot:extension>
        <v-tabs
          v-model="model"
          centered
          slider-color="yellow"
        >
          <v-tab
            :href="`#tab-${i}`"
          >
            INICIO
          </v-tab>
          <v-tab
            :href="`#tab-${i}`"
          >
            CONOCENOS
          </v-tab>
          <v-tab
            :href="`#tab-${i}`"
          >
            CATALOOGOS
          </v-tab>
          <v-tab
            :href="`#tab-${i}`"
          >
            INSTALACIONES
          </v-tab>
          <v-tab
            :href="`#tab-${i}`"
          >
            CONTACTO
          </v-tab>
<v-tab
            :href="`#tab-${i}`"
          >
            BLOG
          </v-tab>
        </v-tabs>
      </template>
    </v-toolbar>
</v-card>
</template>

<script>
export default {

}
</script>

<style>

</style>