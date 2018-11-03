<template>
    <div id="main">
        <navbar></navbar>
        <carousel></carousel>
        <award></award>
        <contact-us></contact-us>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
import Carousel from "./Carousel.vue"
import Award from "./Award.vue"
import ContactUs from "./ContactUs.vue"

export default {
    name: "Main",
  components: {
    "carousel": Carousel,
    "navbar": NavBar,
    "award": Award,
    "contact-us": ContactUs,
  }
}
</script>

<style>
</style>
