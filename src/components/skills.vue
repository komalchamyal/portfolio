<template>

  <div id="resume" class="text-center pt-3 pb-5 mb-3">
    <h1 class="heading display-3">My Skills</h1>

    <br>
    <div class="warpper">
      <input class="radio" id="one" name="group" type="radio" checked>
      <input class="radio" id="two" name="group" type="radio">
      <input class="radio" id="three" name="group" type="radio">

      <div class="tabs">
        <label class="tab" id="one-tab" for="one">Programming</label>
        <label class="tab" id="two-tab" for="two">ML/AI Frameworks</label>
        <label class="tab" id="three-tab" for="three">Data Tools</label>

      </div>
      <div class="panels">
        <div class="panel" id="one-panel">
          <div class="skills-box">
            <div class="container">
              <p class="skill-label">Python</p>
              <div class="skillbar " style="width: 100%; background-color: mediumslateblue;"></div>
            </div>
            <div class="container">
              <p class="skill-label">SQL</p>
              <div class="skillbar" style="width: 100%; background-color: orangered;"></div>
            </div>
            <div class="container">
              <p class="skill-label">R</p>
              <div class="skillbar " style="width: 100%; background-color: 	#f5c10e;"></div>
            </div>
            <div id="resume-link" class="container">
              <p class="skill-label">JavaScript</p>
              <div class="skillbar " style="width: 100%; background-color: indianred;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Java</p>
              <div class="skillbar" style="width: 100%; background-color: green;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Shell Scripting (Bash)</p>
              <div class="skillbar" style="width: 100%; background-color: brown;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Flask + Vue.js</p>
              <div class="skillbar" style="width: 100%; background-color: orange;"></div>
            </div>

          </div>
        </div>
        <div class="panel" id="two-panel">

          <div class="skills-box">
            <div class="container">
              <p class="skill-label">scikit-learn</p>
              <div class="skillbar" style="width: 100%; background-color: orangered;"></div>
            </div>
            <div class="container">
              <p class="skill-label">PyTorch</p>
              <div class="skillbar" style="width: 100%; background-color: palevioletred;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Hugging Face Transformers</p>
              <div class="skillbar" style="width: 100%; background-color: purple;"></div>
            </div>
            <div class="container">
              <p class="skill-label">LangChain </p>
              <div class="skillbar" style="width: 100%; background-color: darkblue;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Azure Machine Learning</p>
              <div class="skillbar " style="width: 100%; background-color: olive;"></div>
            </div>
            <div class="container">
              <p class="skill-label">TensorFlow</p>
              <div class="skillbar " style="width: 100%; background-color: green;"></div>
            </div>
            <div class="container">
              <p class="skill-label">MLflow</p>
              <div class="skillbar" style="width: 100%; background-color: purple;"></div>
            </div>


          </div>
        </div>
        <div class="panel" id="three-panel">

          <div class="skills-box">
            <div class="container">
              <p class="skill-label">Microsoft Fabric</p>
              <div class="skillbar " style="width: 100%; background-color: Purple;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Power BI</p>
              <div class="skillbar " style="width: 100%; background-color: #55c10e;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Apache Spark</p>
              <div class="skillbar " style="width: 100%; background-color: pink;"></div>
            </div>
            <div class="container">
              <p class="skill-label">Databricks</p>
              <div class="skillbar " style="width: 100%; background-color: mediumslateblue;"></div>
            </div>
            <div class="container">
              <p class="skill-label">RDBMS</p>
              <div class="skillbar " style="width: 100%; background-color: rgb(232, 86, 86);"></div>
            </div>
            <div class="container">
              <p class="skill-label">Postman/Insomnia</p>
              <div class="skillbar" style="width: 100%; background-color: #f5c10e;"></div>
            </div>
            <div class="container">
              <p class="skill-label">CI/CD (GitHub Actions, Azure DevOps)</p>
              <div class="skillbar" style="width: 100%; background-color: brown;"></div>
            </div>
          </div>
        </div>
      </div>

    </div>
    <br>
    <div>
      <h2 class="fs-1 subheading ">Certifications</h2>
      <br><br>
      <div class="warpper2">
        <div class="certifications">
          <ol role="list">
            <li><a class="link" target="_blank"
                href="https://learn.microsoft.com/en-us/users/komalchamyal/credentials/7d67236a1cca3432">
                Microsoft Certified: Fabric Data Engineer</a></li>
            <li><a class="link" target="_blank"
                href="https://learn.microsoft.com/en-us/users/komalchamyal/credentials/4f1946f395a046b3">
                Microsoft Certified: Power BI Data Analyst</a></li>
            <li><a class="link" target="_blank"
                href="https://drive.google.com/file/d/1ammzEDdhZFHzPxsVOSOwaezO5dqivkrV/view?usp=sharing">
                IITM Diploma in Programming</a> </li>
            <li><a class="link" target="_blank"
                href="https://drive.google.com/file/d/19C4PkxQNG_doMn1a_DO_fFgYm_rprps3/view?usp=sharing">
                IIT Madras Lead Python Mentor</a> </li>
          </ol>
        </div>
      </div>
    </div>
    <br>
    <div class="text-center">
      <a href="cv.pdf" class="viewcv" data-bs-toggle="tooltip" data-bs-placement="top" title="View Resume"
        target="_blank">
        <h2 class="fs-3 subheading ">Resume</h2>
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

.viewcv .subheading {
  width: 8ch;
  transform: translateY(5px);
}

#resume {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.warpper {
  font-family: 'Poppins', sans-serif;
  display: flex;
  margin: 0ch 2ch;
  flex-direction: column;
  align-items: center;
  min-height: 450px;
}

.warpper2 {
  font-family: 'Poppins', sans-serif;
  display: flex;
  margin: 0ch 2ch;
  flex-direction: column;
  align-items: center;
  min-height: 200px;
  text-align: left;
}

.certifications {
  max-width: 600px;
  font-size: medium;
}

ol {
  list-style: none;
  padding: 0;
}

li+li {
  margin-top: 1rem;
}

li {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1.5rem;
  outline: 1px solid black;
  border-radius: 1rem;
  width: calc(100% - 2rem);
  box-shadow: 0.25rem 0.25rem 0.75rem rgb(0 0 0 / 0.1);
}

li::before {
  counter-increment: list-item;
  content: counter(list-item);
  opacity: 0.85;
  font-size: 2.5rem;
  font-weight: 700;
  width: 1.5em;
  height: 1.5em;
  background: #000000;
  flex: 0 0 auto;
  border-radius: 50%;
  color: rgb(255, 255, 255);
  display: flex;
  outline: 1px solid #000;
  justify-content: center;
  align-items: center;
}

li:nth-child(even) {
  flex-direction: row-reverse;
  margin-right: -2rem;
  margin-left: 2rem;
}

.link {
  color: #3E2723;
  text-decoration: none;
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

.tab:hover,
.tab:checked {
  background: #ffffff;
  color: rgb(0, 0, 0);
  border-bottom: 1px solid rgb(0, 0, 0);
  transform: translateY(-5px);
}


.panels {
  background: transparent;
  min-height: 100px;
  width: 100%;
  max-width: 450px;
  overflow: hidden;
  margin-top: 10px;
  margin-bottom: 5px;
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
  width: 100%;
  flex-wrap: wrap;
}

.skill-label {
  font-size: medium;
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
    width: 95%;
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


  .tab:hover {
    transform: translateX(15px);
  }

  .skill-label {
    font-size: small;
  }

  .certifications {
    font-size: medium;
  }

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
}
</style>
