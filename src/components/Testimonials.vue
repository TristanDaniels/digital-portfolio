<template>
  <section id="testimonials" class="py-5">
    <div class="container text-center">
      <h2 class="mt-3 mb-5 text-white">Testimonials</h2>
    </div>
    <div id="testimonial-slider" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#testimonial-slider"
          data-bs-slide-to="0"
          class="active round-circle"
          style="width: 20px; height: 20px"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#testimonial-slider"
          data-bs-slide-to="1"
          class="round-circle"
          style="width: 20px; height: 20px"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#testimonial-slider"
          data-bs-slide-to="2"
          class="round-circle"
          style="width: 20px; height: 20px"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item pb-5 text-center active">
          <img
            src="https://i.postimg.cc/HxdvMHGw/Raaid.jpg
"
            class="car-img mb-4"
            alt="Raaid"
          />
          <h5 class="text-white">Raaid</h5>
          <p class="text-white">"Man's a big G.O.A.T."</p>
        </div>
        <div class="carousel-item pb-5 text-center">
          <img
            src="https://i.postimg.cc/FKjn1z6F/Joshua.jpg
"
            class="car-img mb-4"
            alt="Joshua"
          />
          <h5 class="text-white">Joshua</h5>
          <p class="text-white">
            Some representative placeholder content for the second slide.
          </p>
        </div>
        <div class="carousel-item pb-5 text-center">
          <img
            src="https://i.postimg.cc/Kvhs2ZVZ/Chanique.jpg"
            class="car-img mb-4"
            alt="Chanique"
          />
          <h5 class="text-white">Chanique</h5>
          <p class="text-white">
            "Tristan is a hardworking individual who always does his utmost best
            in all aspects, always eager to learn and help others whenever and
            wherever he can. Wishing him all the best in his future endeavours."
          </p>
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#testimonial-slider"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#testimonial-slider"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </section>
  <footer id="footer">
    <p class="footer-text">
      <small>© Copyright 2022 Made by Tristan Daniels</small>
    </p>
  </footer>
</template>
<script>
export default {
  name: "Testimonials",
};
</script>
<style scoped>
#testimonials {
  background-image: url(https://i.postimg.cc/59D1rxG4/Background-image.jpg);
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  height: 100vh;
}
.car-img {
  height: 300px;
  width: 250px;
  border-radius: 50px;
}
#footer {
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: black;
  background-color: white;
  padding: 20px;
  font-weight: bold;
}
</style>
