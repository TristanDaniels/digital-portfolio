<template>
  <div class="container mb-3">
    <div class="headings mt-3 mb-3 d-flex justify-content-center">
      <h2>Resume</h2>
    </div>
    <div class="row">
      <div class="col-lg-12">
        <h3 class="resume-title">Summary</h3>
        <div
          class="resume-item shadow border border-5 border-end-0 border-top-0 border-bottom-0 border-primary p-5 pb-0"
        >
          <h4>Tristan Daniels</h4>
          <p>
            <em>
              I am a very optimistic, fun, and loving person. I always try to
              remain positive regardless of how negative the situation can be.
              My passion for technology started when I was a toddler. I would
              always play games on my phone, computers and consoles. I always
              saw myself pursuing a career in I.T because of my interest in it
              since I was young.</em
            >
          </p>
          <ul class="pb-3">
            <li>Western Cape, South Africa</li>
            <li>+27 65 863 4549</li>
            <li>tristandaniels07@gmail.com</li>
          </ul>
        </div>
        <h3 class="resume-title">Education</h3>
        <div
          class="resume-item shadow border border-5 border-end-0 border-top-0 border-bottom-0 border-primary p-5 mb-3"
          v-for="job in resumes"
          :key="job"
        >
          <h4>{{ job.heading }}</h4>
          <h5>{{ job.time }}</h5>
          <p>
            <em>{{ job.loaction }}</em>
          </p>
          <p>{{ job.description }}</p>
        </div>
      </div>
    </div>
  </div>
  <footer id="footer">
    <p class="footer-text">
      <small>© Copyright 2022 Made by Tristan Daniels</small>
    </p>
  </footer>
</template>
<script>
export default {
  name: "Resume",
  data() {
    return {
      resumes: [
        {
          id: 1,
          heading: "Matric Bachelors Pass",
          time: "2017 - 2021",
          location: "Pinelands High",
          description:
            "I spent five years of my life here and didn't once regret the decision I made about wanting to attend Pinelands High. It is an excellent school and I enjoyed my time there. The school played a huge role in molding me into the person I am today.",
        },
        {
          id: 2,
          heading: "Aspiring Fullstack Developer",
          time: "2022 - Present",
          location: "Life Choices Academy",
          description:
            "Learning how to develope and design websites using HTML, CSS and JAVASCRIPT.",
        },
      ],
    };
  },
};
</script>
<style scoped>
#footer {
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: white;
  background-color: black;
  padding: 20px;
  font-weight: bold;
}
</style>
