<template>
    <div id="main">
        <navbar></navbar>
        <carousel></carousel>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
import Carousel from "./Carousel.vue"

export default {
    name: "Main",
  components: {
    "carousel": Carousel,
    "navbar" : NavBar
  }
}
</script>

<style>
</style>
