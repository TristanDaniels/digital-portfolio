<template>
  <section id="landing">
    <h1>I'm Tristan Daniels</h1>
    <h3>Aspiring full-stack web developer</h3>
  </section>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#landing {
  background-image: url(https://i.postimg.cc/t4PGpSR6/Home.jpg);
  background-size: 100%;
  height: 100vh;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  align-content: center;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
}
#landing h1,
#landing h3 {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  color: white;
  font-family: sans-serif;
  text-shadow: 1px 4px 8px black;
}
</style>
