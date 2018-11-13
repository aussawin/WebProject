<template>
    <div id="main">
        <navbar></navbar>
        <carousel></carousel>
        <thirty-years></thirty-years>
        <video-page></video-page>
        <society></society>
        <award></award>
        <contact-us></contact-us>
    </div>
</template>

<script>
import NavBar from './NavBar.vue';
import Carousel from "./Carousel.vue"
import ThirtyYears from './30Years.vue'
import Award from "./Award.vue"
import ContactUs from "./ContactUs.vue"
import Video from "./Video.vue"
import Society from "./Society.vue"

export default {
    name: "Main",
  components: {
    "carousel": Carousel,
    "thirty-years" : ThirtyYears,
    "video-page" : Video,
    "navbar": NavBar,
    "society": Society,
    "award": Award,
    "contact-us": ContactUs,
  }
}
</script>

<style>
</style>
