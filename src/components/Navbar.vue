<template>
  <nav id="Navbar" class="navbar navbar-expand-md">
    <div class="container-lg">
      <!-- navbar brand / title -->
      <a class="navbar-brand" href="#intro">
        <span class="text-dark fw-bold"> Tristan Daniels </span>
      </a>
      <!-- toggle button for mobile nav -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#main-nav"
        aria-controls="main-nav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"
          ><i class="fa-solid fa-bars"></i
        ></span>
      </button>
      <!-- navbar links -->
      <div
        class="collapse navbar-collapse justify-content-end align-center"
        id="main-nav"
      >
        <router-link class="me-2" to="/">Home</router-link>
        <router-link class="me-2" to="/about">About</router-link>
        <router-link class="me-2" to="/resume">Resume</router-link>
        <router-link class="me-2" to="/projects">Projects</router-link>
        <router-link class="me-2" to="/testimonials">Testimonials</router-link>
        <router-link class="me-2" to="/contact">Contact</router-link>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "Navbar",
};
</script>
<style scoped>
#Navbar {
  padding: 20px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  top: 0;
}

nav a {
  font-weight: bold;
  color: black;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #0d6efd;
}
@media screen and (max-width: 768px) {
  nav a {
    display: flex;
    flex-direction: column;
  }
}
</style>
