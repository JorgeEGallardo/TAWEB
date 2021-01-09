<template>
<v-card elevation="17">
  <carousel  paginationSize="35" autoplayTimeout="5000" :navigationEnabled="true" :perPageCustom="[[0, 1]]" :autoplay="true">
  <slide>
    <v-img :src="imgs[0]"></v-img>
  </slide>
  <slide>
    <v-img :src="imgs[1]"></v-img>
  </slide>
  <slide>
    <v-img :src="imgs[2]"></v-img>
  </slide>
</carousel>
</v-card>
</template>
<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
  components: {
    Carousel,
    Slide,
  },
  data () {
      return {
        imgs: [
          require("../../resources/Gal1.jpg"),
          require("../../resources/Gal2.jpg"),
          require("../../resources/Gal3.jpg"),
        ],
      }
      },
  
};
</script>

<style>
.VueCarousel-navigation{
  margin-top:-6rem; 
  }
.VueCarousel-pagination{
  z-index: 2;
}
</style>