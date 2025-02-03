<template>
  <div id="projects" class="text-center mt-3 pt-3">
    <h1 class="heading display-3">Projects</h1>

    <br><br>

    <div class="project-sub">
      <h1 class="display-6">Data Science</h1>
    </div>
    <div class='projects-container'>

      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>Numpy</div>
          <div class='skill'>Pandas</div>
          <div class='skill'>Matplotlib</div>
          <div class='skill'>Seaborn</div>
        </div>
        <img src="data.jpg" />
        <div class='project-card-footer'>
          <p>DATA ANALYSIS</p>
          <p>Performed Data Cleaning, EDA and Visualisation of a car sale dataset of Russia</p>

          <div class="mt-2"><a target="_blank" href="https://github.com/komalchamyal/DAV-Project"
              class="project-icons bi bi-code-slash"></a> <a target="_blank"
              href="https://github.com/komalchamyal/DAV-Project/blob/main/DAV%20project%20CAR%20sales.ipynb"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>

      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>Sklearn</div>
          <div class='skill'>ML Algos</div>
          <div class='skill'>SHAP</div>
          <div class='skill'>Python</div>
          <!-- <div class='skill'>Pandas</div>
          <div class='skill'>Seaborn</div> -->
        </div>
        <img src="ml.webp" />
        <div class='project-card-footer'>
          <p>Big Mart Prediction</p>
          <p>Data Cleaning, EDA, Modelling, Hyperparameter Tuning, Prediction of sales</p>

          <div class="mt-2"><a target="_blank" href="https://github.com/komalchamyal/bigmart-analysis"
              class="project-icons bi bi-code-slash"></a> <a target="_blank"
              href="https://github.com/komalchamyal/bigmart-analysis/blob/main/Big%20Mart%20Pre-processing%20%2B%20Prediction.ipynb"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>
    </div>
    <div class="project-sub">
      <h1 class="display-6">Web Development</h1>
    </div>
    <div class='projects-container'>
      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>Flask</div>
          <div class='skill'>Vue.js</div>
          <div class='skill'>Redis</div>
          <div class='skill'>Celery</div>
        </div>
        <img src="urbanshopper.jpg" />
        <div class='project-card-footer'>
          <p>URBAN SHOPPER</p>
          <p>Grocery app with RBAC and backend jobs.
          </p>
          <div class=""><a href="https://github.com/komalchamyal/grocery-app" target="_blank"
              class="project-icons bi bi-code-slash"></a> <a
              href="https://github.com/komalchamyal/grocery-app" target="_blank"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>
      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>ReactFlow</div>
          <div class='skill'>React</div>
          <div class='skill'>Vite</div>
          <div class='skill'>HTML CSS JS</div>
        </div>
        <img src="mindmap.png" />
        <div class='project-card-footer'>
          <p>MIND MAP</p>
          <p>Import headers from CSV file, Create mind map using nodes and edges and Export it in json
format.
          </p>
          <div class=""><a href="https://github.com/komalchamyal/mind-map" target="_blank"
              class="project-icons bi bi-code-slash"></a> <a
              href="https://my-mind-map.netlify.app/" target="_blank"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>

      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>Python-Flask</div>
          <div class='skill'>Sql-Alchemy</div>
          <div class='skill'>Jinja2</div>
          <div class='skill'>HTML CSS JS</div>
          <div class='skill'>Bootstrap</div>
        </div>
        <img src="quantified.png" />
        <div class='project-card-footer'>
          <p>SELF QUANTIFIED</p>
          <p>Make custom trackers and add logs to them. The application displays the trackers with graphical trendlines.
          </p>
          <div class=""><a href="https://github.com/komalchamyal/SelfQuantified" target="_blank"
              class="project-icons bi bi-code-slash"></a> <a
              href="https://self-quantified-application.komalchamyal.repl.co/" target="_blank"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>

      <div class='project-box'>
        <div class='skill-container'>
          <div class='skill'>Python-Flask</div>
          <div class='skill'>Rest-API</div>
          <div class='skill'>Sql-Alchemy</div>
          <div class='skill'>HTML CSS JS</div>
          <div class='skill'>Bootstrap</div>
          <div class='skill'>Sqlite DB</div>
        </div>
        <img src="kanban.jpg" />
        <div class='project-card-footer'>
          <p>MY KANBAN</p>
          <p>A personalised Kanban board to make boards or lists and add tasks into them. APIs provided with
            documentation.</p>

          <div><a target="_blank" href="https://github.com/komalchamyal/myKanban"
              class="project-icons bi bi-code-slash"></a> <a target="_blank" href="https://MyKanban.komalchamyal.repl.co"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>
    </div>
    <div class="project-sub">
      <h1 class="display-6">Power BI</h1>
    </div>
    <!--
    <div class="projects-container">
      <div class="report-btn">
        <button class="btn btn-dark mx-3" style="width: max-content;" v-if="isHidden1 && isHidden2"
          v-on:click="isHidden1 = false; isHidden2 = true">View Netflix Report</button>   
        <!-- <button class="btn btn-dark mx-3" style="width: max-content;" v-if="isHidden2&&isHidden1"
          v-on:click="isHidden1 = true; isHidden2 = false">View SuperStore Report</button> -->
          <button class="btn btn-dark mx-3" style="width: max-content;" v-else
          v-on:click="isHidden1 = true; isHidden2 = true">Close</button>
      </div>
      <br><br><br>
      <div class="report-space">
        <div class="report" v-if="!isHidden1">
          <iframe class="netflix-report" title="netflix_report" src="https://app.powerbi.com/view?r=eyJrIjoiMWYxMmRlYjctYjRmNi00MDZmLThmZWYtMTg2YWMwYjRiY2I5IiwidCI6ImY5MjMzYTQwLWZiMWEtNDY0ZC1iODVhLTk1OWUzYWI4ZTQ1NCJ9" 
          frameborder="0" allowFullScreen="true" ></iframe></div>

      </div>
    </div> 
  -->


  </div>
</template>

<script>
export default {
  name: 'project-section',
  data() {
    return {
      isHidden1: true,
      isHidden2: true
    };
  }
}
</script>

<style>
.report-btn {
  align-self: center;
  justify-self: center;
  justify-content: center;
}



.netflix-report {
  width: 1200px;
  height: 747px;
}

.project-icons {
  font-size: 20px;
  cursor: pointer;
  color: white;
  background-color: transparent;
  outline: none;
  border: none;
  margin: 5px;
  visibility: hidden;
}

.project-icons:hover {
  color: #92CDCF;
}

#projects {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  max-width: 900px;
  margin: auto;
}

.projects-container {
  margin: 30px;
  min-height: 400px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}

.project-sub {
  align-self: center;
}

.project-box {
  flex-basis: 325px;
  height: 325px;
  margin: 30px 15px;
  border-radius: 5px 5px 0px 0px;
  box-shadow: 3px 2px 17px 0px rgba(50, 50, 50, 0.9);
  background-color: #000000;
  overflow: hidden;
  cursor: pointer;
  transition: 200ms ease-in-out;
}

.skill-container {
  width: 325px;
  height: 150px;
  padding: 10px;
  position: absolute;
  z-index: 10;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  overflow: hidden;
}

.skill {
  display: flex;
  justify-content: center;
  align-items: center;
  align-self: center;
  margin: 10px;
  z-index: 10;
  cursor: default;
  background-color: #1C1D21;
  width: 100px;
  height: 30px;
  font-family: 'Poppins', sans-serif;
  font-size: 15px;
  border-radius: 5px;
  color: #92CDCF;
  opacity: 0;
  transform: translateX(-400px);
  transition: all 0.4s 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.skill:nth-child(2) {
  transform: translateY(-400px);
}

.skill:nth-child(3) {
  transform: translateX(400px);
}

.skill:nth-child(5) {
  transform: translateY(400px);
}

.skill:nth-child(6) {
  transform: translateX(400px);
}

.project-box img {
  width: 100%;
  height: 250px;
  background-color: #EEEFF7;
  object-fit: cover;
  margin: 0px;
  padding: 0px;
  transition: all 0.3s ease-in-out;
}

.project-card-footer {
  font-family: 'Roboto Mono Thin', monospace;
  letter-spacing: 2px;
  width: 100%;
  height: 180px;
  padding: 0 2px;
  background-color: #000000;
  align-self: center;
  color: #bdc3c7;
  transition: all 600ms cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.project-card-footer p {
  padding-top: 30px;
  align-self: center;
  margin-bottom: 0;
  padding-bottom: 0;
  font-size: small;
}

.project-card-footer p:nth-child(2) {
  font-family: 'Roboto Mono', monospace;
  font-size: 12px;

  padding: 5px 15px;
  margin-top: 0px;
  visibility: hidden;
  text-align: center;
}

.project-box:hover {
  cursor: default;
}

.project-box:hover .project-card-footer p {
  padding-top: 10px;
}

.project-box:hover .project-card-footer p:nth-child(2) {
  visibility: visible;
}

.project-box:hover .project-icons {
  visibility: visible;
}

.project-box:hover .project-card-footer {
  transform: translateY(-90px);
  cursor: default;
}

.project-box:hover img {
  filter: grayscale(90%);
  cursor: default;
}

.project-box:hover .skill {
  opacity: 0.9;
  transform: translateX(0px);
}

.skill:hover {
  transition: none;
  color: #fcfdfd;
}

@media (max-width:1224px) {

.netflix-report {
width: 900px;
height: 500px;
}
}

@media (max-width:900px) {

.netflix-report {
width: 600px;
height: 500px;
}
}

@media (max-width:700px) {

  .netflix-report {
  width: 350px;
  height: 500px;
  }

  .project-box {
    flex-basis: 75vw;
    margin: 10% 0;
  }

  .skill-container {
    width: 75vw;
    height: 150px;
  }

  .skill {
    font-size: 14px;
    margin: 0px;
  }

  .project-card-footer {
    font-size: 2vh;
    letter-spacing: 1px;
    width: 100%;
    height: 25vh;
    transform: translateY(-1vh);
  }
}

</style>
