<template>
  <Navbar />
  <router-view />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  components: {
    Navbar,
  },
};
</script>

<style scoped></style>
