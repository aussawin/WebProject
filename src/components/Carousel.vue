<template>
  <div id="carousel">
    <b-carousel style="text-shadow: 1px 1px 2px #333; color: red;" controls indicators background="#ababab"
      :interval="4000" img-width="1024" img-height="480">
      <b-carousel-slide id="slide-img" img-src="../assets/Image/1_Home/BG01.png"></b-carousel-slide>
      <b-carousel-slide id="slide-img" img-src="../assets/Image/1_Home/BG02.png"></b-carousel-slide>
      <b-carousel-slide id="slide-img" img-src="../assets/Image/1_Home/BG03.png"></b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
  export default {
    name: "Carousel",
  }

</script>

<style scoped>
</style>
