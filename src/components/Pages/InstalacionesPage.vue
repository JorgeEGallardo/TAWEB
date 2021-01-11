<template>
  <v-row>
      
    <v-col
      v-for="n in img"
      :key="n"
      class="d-flex child-flex"
      cols="4"
    >
      <v-img
        :src="n"
        :lazy-src="n"
        aspect-ratio="1"
        class="grey lighten-2"
      >
        <template v-slot:placeholder>
          <v-row
            class="fill-height ma-0"
            align="center"
            justify="center"
          >
            <v-progress-circular
              indeterminate
              color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
</template>
<script>
export default {
     data(){
        return{
            img:[
                require("../../resources/1.jpg"),
               require("../../resources/2.jpg"),
               require("../../resources/3.jpg"),
               require("../../resources/4.jpg"),
               require("../../resources/5.jpg"),
               require("../../resources/18.jpg"),
               require("../../resources/7.jpg"),
               require("../../resources/8.jpg"),

                

            ]
        }
    }
}
</script>