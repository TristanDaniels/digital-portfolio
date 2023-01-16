<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12">
        <div class="box-shadow-full">
          <div class="row">
            <div class="col-md-6">
              <div class="row" id="image-info">
                <div class="col-sm-6 col-md-5">
                  <div class="about-img">
                    <img
                      src="https://i.postimg.cc/QCZYCHKX/Tristan.jpg"
                      class="about-img img-fluid rounded b-shadow-a mt-3"
                      style="height: 250px; width: 200px"
                      alt="Picture of me"
                    />
                  </div>
                </div>
                <div class="col-sm-6 col-md-7 h-100">
                  <div class="about-info mt-5">
                    <p class="info">
                      <span class="title-s fw-bold">Name: </span>
                      <span>Tristan Daniels</span>
                    </p>
                    <p class="info">
                      <span class="title-s fw-bold">Profile: </span>
                      <span>Aspiring Full Stack Developer</span>
                    </p>
                    <p class="info">
                      <span class="title-s fw-bold">Email: </span>
                      <span>tristandaniels07@gmail.com</span>
                    </p>
                    <p class="info">
                      <span class="title-s fw-bold">Phone: </span>
                      <span>+27 65 863 4549</span>
                    </p>
                  </div>
                </div>
              </div>
              <div class="skill-mf mb-5">
                <p class="title-s mt-3 fw-bold">Skills</p>
                <span>HTML</span> <span class="pull-right">75%</span>
                <div class="progress mb-3 mt-3">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 75%"
                    aria-valuenow="85"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
                <span>CSS</span> <span class="pull-right">50%</span>
                <div class="progress mb-3 mt-3">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="75"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
                <span>Bootstrap</span> <span class="pull-right">50%</span>
                <div class="progress mb-3 mt-3">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="50"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
                <span>JavaScript</span> <span class="pull-right">20%</span>
                <div class="progress mt-3">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 20%"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
            </div>
            <div class="col-md-6">
              <div class="about-me pt-4 pt-md-0 mt-3">
                <div class="title-box-2">
                  <h2 class="title-left mb-4">About me</h2>
                </div>
                <p class="lead">
                  I'm an aspiring full-stack web developer working at LC studio.
                  I'm always willing to learn and focus on the task at hand. I
                  strive to do my best no matter the circumstances.
                </p>
                <p class="lead">
                  I like to play sports such as football, tennis and cricket. I
                  enjoy going outdoors whether it's hiking, camping or exploring
                  places I haven't been to before. I love socialising with my
                  friends and spending time with my loved-ones.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <footer id="footer">
    <p class="footer-text">
      <small>© Copyright 2023 Made by Tristan Daniels</small>
    </p>
  </footer>
</template>
<script>
export default {
  name: "About",
};
</script>
<style scoped>
.container {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.about-img {
  object-fit: cover;
}
#footer {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: white;
  background-color: black;
  padding: 20px;
  font-weight: bold;
}
</style>
