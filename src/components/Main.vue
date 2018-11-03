<template>
    <div id="main">
        <navbar></navbar>
        <carousel></carousel>
        <contact-us></contact-us>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
import Carousel from "./Carousel.vue"
import ContactUs from "./ContactUs.vue"

export default {
    name: "Main",
  components: {
    "carousel": Carousel,
    "navbar": NavBar,
    "contact-us": ContactUs,
  }
}
</script>

<style>
</style>
