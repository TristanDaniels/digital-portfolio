<template>
  <section class="container">
    <div>
      <h2>Projects</h2>
    </div>
    <div class="mt-3 mb-5">
      <div id="projects" class="project-container">
        <div class="template" v-for="project in projects" :key="project">
          <img
            data-bs-toggle="modal"
            :data-bs-target="'#project' + project.id"
            :src="project.image"
            alt="Project"
            class="project"
          />
          <!-- Modals -->
          <div
            class="modal fade"
            :id="'project' + project.id"
            tabindex="-1"
            aria-labelledby="exampleModalLabel"
            aria-hidden="true"
          >
            <div class="modal-dialog">
              <div class="modal-content">
                <div class="modal-header">
                  <h5 class="modal-title" :id="'project' + 'project.id'">
                    {{ project.name }}
                  </h5>
                  <button
                    type="button"
                    class="btn-close"
                    data-bs-dismiss="modal"
                    aria-label="Close"
                  ></button>
                </div>
                <div class="modal-body">
                  <img
                    :src="project.image"
                    class="img-fluid me-3 mb-2"
                    style="width: 100%"
                  />
                  <p>{{ project.description }}</p>
                </div>
                <div class="modal-footer">
                  <button type="button" class="btn btn-secondary">
                    <a :href="project.github"
                      ><span class="text-white">Github</span></a
                    >
                  </button>
                  <button type="button" class="btn btn-primary">
                    <a :href="project.website"
                      ><span class="text-white">Open</span></a
                    >
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <footer id="footer">
    <p class="footer-text">
      <small>© Copyright 2023 Made by Tristan Daniels</small>
    </p>
  </footer>
</template>
<script>
export default {
  name: "Projects",
  data() {
    return {
      projects: [
        {
          id: 1,
          image: "https://i.postimg.cc/6q3vXLcF/Property.jpg",
          name: "Propertz",
          description:
            "A property listing website where you can filter and find the best suited home for you.",
          github: "https://github.com/TristanDaniels/Property-listings.git",
          website: "https://tristans-property-listings.netlify.app/",
        },
        {
          id: 2,
          image: "https://i.postimg.cc/y8TqtwQQ/BMI-calculator.jpg",
          name: "BMI-calculator",
          description: "A website where you can calculate your BMI.",
          github: "https://github.com/TristanDaniels/BMI-Calculator.git",
          website: "https://tristans-bmi-calculator.netlify.app/",
        },
        {
          id: 3,
          image: "https://i.postimg.cc/CxnGkWP6/Calculator.jpg",
          name: "Calculator",
          description: "A working calculator made with JavaScript.",
          github: "https://github.com/TristanDaniels/Calculator.git",
          website: "https://tristandanielscalculator.netlify.app/",
        },
        {
          id: 4,
          image: "https://i.postimg.cc/59FXRHdb/Mock-portfolio.jpg",
          name: "Mock Portfolio",
          description: "A mock portfoilio built using HTML and CSS.",
          github: "https://github.com/TristanDaniels/Digital-CV.git",
          website: "https://tristandaniels.netlify.app/",
        },
        {
          id: 5,
          image: "https://i.postimg.cc/fbmGWnPm/tcd-gaming.jpg",
          name: "TCD Gaming",
          description: "A full stack website built using Vue.js and MySQL",
          github: "https://github.com/TristanDaniels/tcd-gaming.git",
          website: "https://tcd-gaming.netlify.app/",
        },
        {
          id: 6,
          image: "https://i.postimg.cc/CxNCxcNF/Restaurant.jpg",
          name: "Restaurant",
          description:
            "A website displayng a home page and about page for a restaurant.",
          github: "https://github.com/TristanDaniels/Restaurant.git",
          website: "https://restaurantlyattempt.netlify.app/",
        },
      ],
    };
  },
};
</script>
<style scoped>
.container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
h2 {
  display: flex;
  justify-content: center;
}
#projects {
  display: flex;
  align-content: center;
  justify-content: center;
  text-align: center;
  flex-direction: row;
  align-items: center;
  flex-wrap: wrap;
}
.project-container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  text-align: center;
  gap: 20px;
}
.template {
  padding-top: 20px;
  padding-left: 20px;
  padding-right: 20px;
}
.template img {
  width: 372px;
  height: 250px;
  object-fit: cover;
}
#footer {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-end;
  color: white;
  background-color: black;
  padding: 20px;
  font-weight: bold;
  bottom: 0;
  width: 100%;
}
@media screen and (max-width: 700px) {
  .project-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
@media screen and (max-width: 410px) {
  .template img {
    width: 250px;
  }
}
</style>
