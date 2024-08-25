<template>


  <div id="about" ref="about" class="text-center pt-1">
    <h1 class="heading display-3 mt-5" style="color:black">About Me</h1>
    <div class="info">
      <img src="new1.jpg" class="image-fluid imgs" />
      <div class="intro ">
        I'm a Passionate and Results-Driven Professional in Business and Technology.
        I specialize in problem solving. That has made me a fundamental expert in machine learning, data analysis, modelling and client services/relations. I’m known for applying technical expertise as well as business knowledge to drive impactful projects. 
        Technology intrigues me and I really enjoy using whatever skills I have to solve day-to-day problems with code. <br>I have completed my
        Bachelor's from Hansraj College, Delhi University with Computer Science major. I have also done Diploma in Programming from IIT Madras. I have experience working at a startup for 1+ yr as a Data Scientist and Data Analyst. <br> Currently Building my own AI powered Plants business.
        Outside of work, I enjoy <a href="https://www.instagram.com/komaldanx/" target="_blank" class="danx">dancing</a>, swimming, traveling, and spending time with my loved ones :)
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
    padding-top: 5%;
    padding-bottom: 5%;
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
