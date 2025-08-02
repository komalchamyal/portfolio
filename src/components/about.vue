<template>


  <div id="about" ref="about" class="text-center pt-1">
    <h1 class="heading display-3 mt-5" style="color:black">About Me</h1>
    <div class="info">
      <img src="pic.jpg" class="image-fluid imgs" />
      <div class="intro text-center">
        <h2 class="fs-6 ">Skills from the Hills: Data, Dance & Debugging</h2><br>
A data nerd with roots in nature and a thing for machine learning. With a CS degree from Hansraj College and a Programming Diploma from IIT Madras, I blend algorithms with business sense to build real-world AI solutions.

Currently an Associate Data Scientist at <a href="https://www.proarch.com/" target="_blank" class="danx">ProArch</a>, where I build and deploy ML models, explore LLMs, and try not to overfit — both in code and in life.

Endlessly learning, always collaborating, and never too far from a dance floor, swimming pool, or a hot cup of chai.
      </div>
      <img src="pic4.jpg" class="imgs" />

    </div>
</div>

</template>

<script>
export default {
  name: 'about-section',
  props: {
    msg: String
  }
}

</script>

<style>
.danx{
  color: #000000;
}
.danx:hover{
  color: #ffffff;
}

#about{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-height: 90vh;
}

.info {
  text-align: center;
  display: flex;
  margin: 5%;
  align-self:center;

}

.intro {
  font-family: 'Poppins', sans-serif;
  padding: 5%;
  width: 70%;
  text-align: left;
  font-size: large;
}

@media (max-width: 1300px) {
  .info {
    flex-direction: column;
    align-content: center;
  }

  .intro {
    padding-left: 10%;
    padding-right: 10%;
/*     padding-top: 5%;
    padding-bottom: 5%; */
    width: 100%;
    font-size: medium;
  }

  .imgs {
    align-self: center;
    border-radius: 25px;
    max-height: 200px;
    max-width: 250px;
    transform: scale(0.95);
    margin: 2ch;
    box-shadow: palevioletred 1rem 1rem 1rem;
  }
}

.collage {
  display: flex;
  flex-direction: column;
}

.imgs {
  border-radius: 25px;
  max-height: 40vh;
  max-width: 40vw;
  transform: scale(0.95);
  margin: 2ch;
  z-index: 100;
  box-shadow: rgb(160, 142, 142) 1rem 1rem 1rem;
}

.imgs:hover {
  transform: scale(1);
}


</style>
