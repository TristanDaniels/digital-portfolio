<template>
  <div class="container project-container">
    <div class="template">
      <img
        data-bs-toggle="modal"
        data-bs-target="#project1"
        src="Book.jpg"
        alt="Project 1"
        class="project"
      />
    </div>
    <div class="template">
      <img
        data-bs-toggle="modal"
        data-bs-target="#project2"
        src="Maldives.jpg"
        alt="Project 2"
        class="project"
      />
    </div>
    <div class="template">
      <img
        data-bs-toggle="modal"
        data-bs-target="#project3"
        src="Restaurant 2.jpg"
        alt="Project 3"
        class="project"
      />
    </div>
  </div>
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
          <h5 class="modal-title" id="project1">Buy my book(demo)</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img src="Book.jpg" class="img-fluid me-3 mb-2" style="width: 100%" />
          <p>
            A project built using Bootstrap. Template of a website where a book
            is being sold.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/Bootstrap.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href="https://bootstrapattempt.netlify.app/"
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
          <h5 class="modal-title" id="project2">Calculator</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img
            src="Maldives.jpg"
            class="img-fluid me-3 mb-2"
            style="width: 100%"
          />
          <p>
            One of my beginner projects that links the home page to a contact
            page.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/Holiday-Destination.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href=""><span class="text-white">Open</span></a>
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
          <h5 class="modal-title" id="project3">Restaurant</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <img
            src="Restaurant 2.jpg"
            class="img-fluid me-3 mb-2"
            style="width: 100%"
          />
          <p>
            Incomplete project but showcases a working navbar with a striking
            appearance.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary">
            <a href="https://github.com/TristanDaniels/Restaurant.git"
              ><span class="text-white">Github</span></a
            >
          </button>
          <button type="button" class="btn btn-primary">
            <a href="https://restaurantlyattempt.netlify.app/"
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
<style scoped></style>
