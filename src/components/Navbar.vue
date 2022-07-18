<template>
  <nav id="Navbar">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/resume">Resume</router-link>
    <router-link to="/projects">Projects</router-link>
    <router-link to="/testimonials">Testimonials</router-link>
    <router-link to="/contact">Contact</router-link>
  </nav>
</template>
<script>
export default {
  name: "Navbar",
};
</script>
<style scoped>
#Navbar {
  padding: 30px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: black;
}
</style>
