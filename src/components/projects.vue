<template>
  <div id="projects" class="text-center mt-3 pt-3">
    <h1 class="heading display-1">Projects</h1>

    <div class='projects-container'>
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
          <div><a href="https://github.com/komalchamyal/SelfQuantified" target="_blank" class="project-icons bi bi-code-slash"></a> <a
              href="https://self-quantified-application.komalchamyal.repl.co/" target="_blank"
              class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>
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

          <div><a target="_blank" href="https://github.com/komalchamyal/DAV-Project" class="project-icons bi bi-code-slash"></a> <a
            target="_blank" href="https://github.com/komalchamyal/DAV-Project/blob/main/DAV%20project%20CAR%20sales.ipynb"
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

          <div><a target="_blank" href="https://github.com/komalchamyal/myKanban" class="project-icons bi bi-code-slash"></a> <a
            target="_blank" href="https://MyKanban.komalchamyal.repl.co" class="project-icons bi bi-box-arrow-up-right"></a>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class='projects-container'>
    </div> -->


  </div>

</template>

<script>
export default {
  name: 'project-section'
}
</script>

<style>
.project-icons {
  font-size: 25px;
  cursor: pointer;
  color: white;
  background-color: transparent;
  outline: none;
  border: none;
  margin: 2px;
  visibility: hidden;
  /* transition: 100ms ease-in-out; */
  /* box-shadow: 0px 0px 12px white ; */
}

.project-icons:hover {
  color: #92CDCF;
}

#projects {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.projects-container {
  margin: 30px;
  min-height: 400px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}

.project-box {
  flex-basis: 375px;
  height: 375px;
  margin: 10px 5px;
  border-radius: 5px 5px 0px 0px;
  box-shadow: 3px 2px 17px 0px rgba(50, 50, 50, 0.9);
  background-color: #000000;
  overflow: hidden;
  cursor: pointer;
  transition: 200ms ease-in-out;
}

.skill-container {
  width: 375px;
  height: 215px;
  padding: 10px;
  position: absolute;
  z-index: 10;
  display: flex;
  flex-wrap: wrap;
  /* margin: 0 37px; */
  justify-content: space-around;
  /* align-items: center ; */
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
  /* overflow: visible; */
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
  height: 275px;
  background-color: #EEEFF7;
  object-fit: cover;
  margin: 0px;
  padding: 0px;
  transition: all 0.3s ease-in-out;
}

.project-card-footer {
  font-family: 'Roboto Mono Thin', monospace;
  font-size: 15px;
  letter-spacing: 2px;
  width: 100%;
  height: 180px;
  transform: translateY(-10px);
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
  font-size: large;
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

.project-box:hover .project-card-footer p:nth-child(2),
.project-box:hover .project-icons {
  visibility: visible;
}

.project-box:hover .project-card-footer {
  transform: translateY(-65px);
  cursor: default;
}

.project-box:hover img {
  filter: grayscale(70%);
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


@media (max-width:500px) {
  .project-box {
    flex-basis: 80vw;
    margin: 10% 0;
  }

  .skill-container {
    width: 80vw;
    height: 180px;
    padding: 10px;
  }

  .skill {
    font-size: 14px;
  }

  .project-card-footer {
    font-size: 2vh;
    letter-spacing: 1px;
    width: 100%;
    height: 25vh;
    transform: translateY(-1vh);
  }

  /*
.project-box:hover .project-card-footer {
transform: translateY(-5vh);
cursor: default;
} */

  .project-card-footer p:nth-child(2) {
    font-size: 11px;
  }
}

@media (max-width:360px) {

  .skill-container {
    width: 80vw;
    height: 160px;
    padding: 10px;
  }

  .project-box {
    flex-basis: 100%;
    /* width: 100vw; */
    margin: 10% 0;
  }

  .project-card-footer {
    font-size: 1vh;
    letter-spacing: 1px;
    width: 100%;
    height: 27vh;
    /* transform: translateY(-10vh); */
  }


  .project-box:hover .project-card-footer {
    transform: translateY(-13vh);
    cursor: default;
  }

  .project-card-footer p:nth-child(2) {
    font-size: 11px;
  }
}
</style>