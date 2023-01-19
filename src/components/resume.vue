<template>

  <div id="resume" class="text-center pt-3 pb-5 mb-3">
    <h1 class="heading display-1">My Skills</h1>


    <div class="warpper">
      <input class="radio" id="one" name="group" type="radio" checked>
      <input class="radio" id="two" name="group" type="radio">
      <input class="radio" id="three" name="group" type="radio">

      <div class="tabs">
        <label class="tab" id="one-tab" for="one">Programming</label>
        <label class="tab" id="two-tab" for="two"> Web Dev</label>
        <label class="tab" id="three-tab" for="three"> More</label>

      </div>
      <div class="panels">
        <div class="panel" id="one-panel">
          <div class="skills-box">
            <div class="container">
              <p class="skill-label">Python</p>
              <div class="skillbar " style="width: 97%; background-color: mediumslateblue;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Java</p>
              <div class="skillbar" style="width: 87%; background-color: orangered;"></div>
            </div>
            <div class="container">
              <p class="skill-label">C++</p>
              <div class="skillbar " style="width: 85%; background-color: 	#f5c10e;"></div>
            </div>
            <div  id="resume-link" class="container">
              <p class="skill-label">SQL</p>
              <div class="skillbar " style="width: 92%; background-color: indianred;"></div>
            </div>
            <div class="container">
              <p class="skill-label">R</p>
              <div class="skillbar" style="width: 85%; background-color: green;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Linux</p>
              <div class="skillbar" style="width: 89%; background-color: brown;"></div>
            </div>

          </div>
        </div>
        <div class="panel" id="two-panel">

          <div class="skills-box">
            <div class="container">
              <p class="skill-label">Vue.js</p>
              <div class="skillbar" style="width: 92%; background-color: orangered;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Flask</p>
              <div class="skillbar" style="width: 92%; background-color: palevioletred;"></div>
            </div>
            <div class="container">
              <p class="skill-label">HTML</p>
              <div class="skillbar " style="width: 95%; background-color: olive;"></div>
            </div>
            <div class="container">
              <p class="skill-label">CSS</p>
              <div class="skillbar" style="width: 95%; background-color: 	#f5c00b;"></div>
            </div>
            <div class="container">
              <p class="skill-label">JavaScript</p>
              <div class="skillbar " style="width: 90%; background-color: green;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Bootstrap</p>
              <div class="skillbar" style="width: 93%; background-color: purple;"></div>
            </div>

          </div>
        </div>
        <div class="panel" id="three-panel">

          <div class="skills-box">
            <div class="container">
              <p class="skill-label">SQL-Alchemy</p>
              <div class="skillbar" style="width: 95%; background-color: 	darkblue;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Data Visualisation: Matplotlib, Seaborn</p>
              <div class="skillbar " style="width: 90%; background-color: #55c10e;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Data Structures & Algorithms</p>
              <div class="skillbar" style="width: 94%; background-color: orange;"></div>
            </div>
            <div class="container">
              <p class="skill-label">REST API</p>
              <div class="skillbar" style="width: 95%; background-color: 	purple;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Numpy, Pandas</p>
              <div class="skillbar" style="width: 90%; background-color: #f5c10e;"></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div  class="text-center">
      <!-- <object data="cv.pdf" class="image-fluid" width="700" height="400"></object> -->
      <a href="cv.pdf" class="viewcv" data-bs-toggle="tooltip" data-bs-placement="top" title="View Resume" target="_blank">
        <h2 class="fs-2 subheading ">Resume</h2>
      </a>
      <a href="cv.pdf" download="KomalChamyalCV">
        <button class="btn btn mx-4 btn-outline-dark" data-bs-toggle="tooltip" data-bs-placement="top"
          title="Download Resume"><i class="bi bi-download"></i></button>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'resume-section',
  props: {
    msg: String
  }
}

</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap");
.viewcv .subheading{
  width: 8ch;
  transform: translateY(5px);
}

#resume{
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.warpper {
  font-family: 'Poppins', sans-serif;
  display: flex;
  margin: 4ch;
  flex-direction: column;
  align-items: center;
}

.tab {
  cursor: pointer;
  padding: 1ch 1ch;
  margin: 2px 2px;
  background: #000000;
  display: inline-block;
  color: #fff;
  border: 1px;
  border-radius: 3px 3px 0px 0px;
  transition: all 0.1s ease-in-out;
}

.tab:hover {
  background: #ffffff;
  color: rgb(0, 0, 0);
  border-bottom: 1px solid rgb(0, 0, 0);
  transform: translateY(-5px);

}

.panels {
  background: transparent;
  min-height: 100px;
  width: 100%;
  max-width: 700px;
  overflow: hidden;
  padding-bottom: 3.5ch;
}

.panel {
  display: none;
  animation: fadein 0.8s;
}

@keyframes fadein {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

.radio {
  display: none;
}

#three:checked~.panels #three-panel,
#two:checked~.panels #two-panel,
#one:checked~.panels #one-panel {
  display: block;
}

#two:checked~.tabs #two-tab,
#three:checked~.tabs #three-tab,
#one:checked~.tabs #one-tab {
  background: #ffffff;
  color: rgb(0, 0, 0);
  border-bottom: 1px solid #000000;

  box-shadow: #000 0 0.1rem 0.1rem;
  overflow: visible;
}

.skills-box {
  display: flex;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
  flex-wrap: wrap;
}

.skill-label {
  font-size: larger;
  font-weight: 500;
  margin: 0;
  margin-top: 2ch;
  padding: 0;
}

@media (max-width:578px) {
  .skills-box {
    display: flex;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
    flex-wrap: wrap;
  }


  .tab {
    cursor: pointer;
    padding: 1ch 1ch;
    font-size: small;
    margin-top: 2px;
    background: #000000;
    display: inline-block;
    color: #fff;
    border-radius: 3px 3px 0px 0px;
    width: 70%;
  }
.skill-label {
  font-size: medium;}

}

.container {
  width: 100%;
  background-color: transparent;
  text-align: center;
}

.skillbar {
  padding-top: 4px;
  padding-bottom: 2px;
  color: white;
  box-shadow: #6a6060 2px 2px 2px;
}

#resume,
#contact,
#projects {
  min-height: 100vh;
  /* background-image: url('../../public/bg3.webp'); */
}
</style>