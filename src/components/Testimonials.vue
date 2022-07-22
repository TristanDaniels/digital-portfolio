<template>
  <section id="testimonials" class="py-5">
    <div class="container text-center">
      <h2 class="mt-3 mb-5 text-white">Testimonials</h2>
    </div>
    <div id="testimonial-slider" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-indicators">
        <button
          v-for="(testimonial, index) in testimonials"
          :key="testimonial.id"
          type="button"
          data-bs-target="#testimonial-slider"
          :data-bs-slide-to="index"
          :class="{ active: index === 0 }"
          class="round-circle"
          style="width: 20px; height: 20px"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
      </div>
      <div class="carousel-inner">
        <div
          class="carousel-item pb-5 text-center"
          :class="{ active: index === 0 }"
          v-for="(testimonial, index) in testimonials"
          :key="testimonial.id"
        >
          <img :src="testimonial.image" class="car-img mb-4" alt="Raaid" />
          <h5 class="text-white">{{ testimonial.name }}</h5>
          <p class="testimonial text-white">"{{ testimonial.testimonial }}"</p>
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
  data() {
    return {
      testimonials: [
        {
          id: 1,
          image: "https://i.postimg.cc/HxdvMHGw/Raaid.jpg",
          name: "Raaid",
          testimonial: "Man's a big G.O.A.T.",
        },
        {
          id: 2,
          image: "https://i.postimg.cc/FKjn1z6F/Joshua.jpg",
          name: "Joshua",
          testimonial:
            "Tristan is a self-motivated, dedicated and authentic individual. I consider him to be a great asset to any workplace due to his outspoken personality and charisma.",
        },
        {
          id: 3,
          image: "https://i.postimg.cc/Kvhs2ZVZ/Chanique.jpg",
          name: "Chanique",
          testimonial:
            "Tristan is a hardworking individual who always does his utmost best in all aspects, always eager to learn and help others whenever and wherever he can. Wishing him all the best in his future endeavours.",
        },
        {
          id: 4,
          image: "https://i.postimg.cc/L8wwFR9c/Abdool-Zaid.jpg",
          name: "Abdul",
          testimonial:
            "Tristan is a kind soul who can easily form the backbone of any team  he is dedicated to his craft and shows great work ethic",
        },
        {
          id: 5,
          image: "https://i.postimg.cc/5yzmtCqB/jason.jpg",
          name: "Jason",
          testimonial:
            "Tristan seems to be a very consistent developer. He gets quite excited when he sees an opportunity to participate and show off his abilities. I'm always happy to see him determined to do well on his projects. He is always challenging himself to write complex ideas for his own level to challenge his coding skills. As long as he is focused, Tristan will continue to do well.",
        },
        {
          id: 6,
          image: "https://i.postimg.cc/MHfRGn99/Cameron-1.jpg",
          name: "Cameron",
          testimonial:
            "Tristan is a very competent individual, he strives higher than what he is capable of doing. His passion for his work preference is outstanding and he is a headstrong and smart working personS",
        },
      ],
    };
  },
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
  object-fit: cover;
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
