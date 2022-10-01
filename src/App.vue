<template>
  <Header />
  <Trips />
  <Gallery />
  <Contact />
</template>
<script>
import Header from "./components/Header.vue";
import Trips from "./components/Trips.vue";
import Gallery from "./components/Gallery.vue";
import Contact from "./components/Contact.vue";
export default {
  name: "App",
  components: {
    Header,
    Trips,
    Gallery,
    Trips,
    Contact,
  },
};
</script>
<style></style>
