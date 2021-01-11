<template>
<div style="min-heigth:78vh">
    <v-row>
        <v-col style="margin:auto" cols="12" md="8"><v-img @click="openPDF" :src="img"></v-img></v-col>
    </v-row>
</div>
</template>
<script>
export default {
     data(){
        return{
            img:require("../../resources/tornillos portada.png"),
        }
    },methods:{
        openPDF(){
            window.location.replace("https://tornillosaguila.vir.mx/catalogo/");
        }
    }
}
</script>
<style scoped>

</style>