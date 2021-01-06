<template>
<div>
    <h1>aassaaa</h1>
  <carousel :perPageCustom="[[0, 1]]" :autoplay="true">
  <slide>
    Slide 1 Content
  </slide>
  <slide>
    Slide 2 Content
  </slide>
</carousel>
</div>
</template>
<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
  components: {
    Carousel,
    Slide
  }
};
</script>

<style>

</style>