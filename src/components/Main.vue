<template>
    <div id="main">
        <navbar></navbar>
        <carousel></carousel>
        <thirty-years></thirty-years>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
import Carousel from "./Carousel.vue"
import ThirtyYears from './30Years.vue'

export default {
    name: "Main",
  components: {
    "carousel": Carousel,
    "navbar" : NavBar,
    "thirty-years" : ThirtyYears
  }
}
</script>

<style>
</style>
