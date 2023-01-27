<template>
  <section
    id="contact"
    data-aos="fade-up"
    data-aos-offset="500"
    class="container"
  >
    <div class="form mt-3">
      <h2 class="mb-5">Contact me</h2>
      <form class="form" action="https://formspree.io/f/xjvdvlew" method="POST">
        <div class="mb-3">
          <label class="form-label">Name</label>
          <input type="text" class="form-control" name="name" />
        </div>
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label"
            >Email address</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleInputEmail1"
            aria-describedby="emailHelp"
            name="email"
          />
          <div class="form-text">
            We'll never share your email with anyone else.
          </div>
        </div>
        <div class="mb-3">
          <label class="form-label">Date</label>
          <input type="date" class="form-control" name="date" />
        </div>
        <div class="mb-3">
          <label class="form-label">Message</label>
          <textarea
            class="form-control"
            style="width: 50%"
            name="message"
          ></textarea>
        </div>
        <div id="btn" class="btn-container d-flex justify-content-center">
          <button type="submit" class="button btn btn-primary mb-5">
            Submit
          </button>
        </div>
      </form>
    </div>
    <div class="text-container">
      <div
        class="paragraph d-flex flex-column justify-content-center align-items-center"
      >
        <h2>Get in touch</h2>
        <p>
          Feel free to contact me with the information provided below. I will
          try to respond to queries and possible collaborations as fast as
          possible. I look forward to working with you.
        </p>
      </div>
      <diV class="communication mb-4 pb-3">
        <ul class="list">
          <li>Cape Town</li>
          <li>+27 65 863 4549</li>
          <li>tristandaniels07@gmail.com</li>
        </ul>
      </diV>
      <div class="socials">
        <ul>
          <li class="icons">
            <a href="https://www.linkedin.com/in/tristan-daniels-78425a23a/"
              ><i class="fa-brands fa-linkedin"></i
            ></a>
          </li>
          <li class="icons">
            <a href="https://github.com/TristanDaniels"
              ><i class="fa-brands fa-github"></i>
            </a>
          </li>
        </ul>
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
  name: "Contact",
};
</script>
<style scoped>
#contact {
  display: flex;
  flex-direction: column;
  gap: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.form {
  width: 100%;
}
input {
  width: 50%;
  display: flex !important;
  justify-content: center !important;
  align-content: center;
}
.mb-3 {
  margin-bottom: 1rem !important;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.form-label {
  display: flex;
  justify-content: center;
  align-items: center;
}
.form-text {
  display: flex;
  justify-content: center;
  align-items: center;
}
#contact h2 {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.label {
  display: flex;
  flex-direction: column;
  color: black;
  font-family: sans-serif;
}
.submit {
  display: flex;
  flex-direction: row;
  justify-content: center;
  font-family: sans-serif;
  width: 100%;
}
.text-container {
  width: 50%;
  margin-bottom: 40px;
}
.text-container p {
  color: black;
  font-family: sans-serif;
}
.communication {
  margin-top: 40px;
  font-family: sans-serif;
  display: flex;
  justify-content: center;
  align-content: center;
}
.socials {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-end;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.list {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.icons {
  display: inline;
  padding: 10px;
  font-size: 30px;
}
#footer {
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: white;
  background-color: black;
  padding: 20px;
  font-weight: bold;
  bottom: 0;
  width: 100%;
}
@media screen and (max-width: 700px) {
  #contact {
    display: flex;
    flex-direction: column;
  }
}
</style>
