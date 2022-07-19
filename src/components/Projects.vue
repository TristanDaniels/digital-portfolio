<template>
  <section id="projects" class="container mb-5">
    <h2>Projects</h2>
    <div class="project-container">
      <div class="template">
        <img
          data-bs-toggle="modal"
          data-bs-target="#project1"
          src="https://i.postimg.cc/CxnGkWP6/Calculator.jpg"
          alt="Project 1"
          class="project"
        />
      </div>
      <div class="template">
        <img
          data-bs-toggle="modal"
          data-bs-target="#project2"
          src="https://i.postimg.cc/qRyS4ybB/Property.jpg"
          alt="Project 2"
          class="project"
        />
      </div>
      <div class="template">
        <img
          data-bs-toggle="modal"
          data-bs-target="#project3"
          src="https://i.postimg.cc/y8TqtwQQ/BMI-calculator.jpg"
          alt="Project 3"
          class="project"
        />
      </div>
    </div>
  </section>
  <footer id="footer">
    <p class="footer-text">
      <small>© Copyright 2022 Made by Tristan Daniels</small>
    </p>
  </footer>
  <!-- Button trigger modal -->
  <!-- Modals -->
  <div
    class="modal fade"
    id="project1"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="project1">Calculator</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img
            src="https://i.postimg.cc/CxnGkWP6/Calculator.jpg"
            class="img-fluid me-3 mb-2"
            style="width: 100%"
          />
          <p>A working calculator made with JavaScript.</p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/Calculator.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href="https://tristandanielscalculator.netlify.app/"
              ><span class="text-white">Open</span></a
            >
          </button>
        </div>
      </div>
    </div>
  </div>

  <div
    class="modal fade"
    id="project2"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="project2">Propertz</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img
            src="https://i.postimg.cc/6q3vXLcF/Property.jpg"
            class="me-3 mb-2"
            style="width: 100%"
          />
          <p>
            A property listing website where you can filter and find the best
            suited home for you.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/Property-listings.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href="https://tristans-property-listings.netlify.app/"
              ><span class="text-white">Open</span></a
            >
          </button>
        </div>
      </div>
    </div>
  </div>

  <div
    class="modal fade"
    id="project3"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="project3">BMI Calculator</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img
            src="https://i.postimg.cc/y8TqtwQQ/BMI-calculator.jpg"
            class="img-fluid me-3 mb-2"
            style="width: 100%"
          />
          <p>A website where you can calculate your BMI.</p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/BMI-Calculator.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href="https://tristans-bmi-calculator.netlify.app/"
              ><span class="text-white">Open</span></a
            >
          </button>
        </div>
      </div>
    </div>
  </div>
  <!-- End of Modal -->
</template>
<script>
export default {
  name: "Projects",
};
</script>
<style scoped>
#projects {
  display: flex;
  align-content: center;
  justify-content: center;
  text-align: center;
  flex-direction: column;
  align-items: center;
}
.project-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  flex-wrap: wrap;
}
.template {
  width: 100%;
  padding-top: 20px;
  padding-left: 20px;
  padding-right: 20px;
}
.project {
  width: 30%;
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
}
@media screen and (max-width: 700px) {
  .project-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
