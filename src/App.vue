/* eslint-disable */
<template>
  <div>
    <Navbar />
    <Body />
    <Caroussel />
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Body from "./components/Body";
import Caroussel from "./components/Caroussel.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Body,
    Caroussel,
    Footer,
  },
};
</script>
