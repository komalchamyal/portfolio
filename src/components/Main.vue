<template>

  <div class="wrapper">
    <!-- profile picture -->
    <div class="myimg mt-1">
      <img alt="My picture"
        class="myimg mx-auto shadow-lg image-fluid animate__animated animate__fadeInUp"
        :src="'vector.jpg'">
    </div>
    <!-- Typing Intro -->
    <div class="typing-text fs-2 mx-3">
      Hi, I am Komal Chamyal!
    </div>
    <!-- Links to sections -->
    <div class="buttons animate__animated animate__fadeInDown">
      <button onclick="scrolldiv('about')" class="button-28 fs-6" role="button">About</button>
      <button onclick="scrolldiv('projects')" class="button-28 fs-6" role="button">Projects</button>
      <button onclick="scrolldiv('resume')" class="button-28 fs-6" role="button">Skills</button>
      <button type="submit" onclick="window.open('cv.pdf')" class="button-28 fs-6" data-bs-toggle="tooltip" data-bs-placement="top" title="View Resume"  role="button">CV
      <i class="bi bi-link-45deg"></i></button>
      <button onclick="scrolldiv('contact')" class="button-28 fs-6" role="button">Contact</button>
    </div>

    <!-- bottom fixed navbar  -->
    <nav class="navbar fixed-bottom navbar-expand" style="background-color: transparent;">
      <div class="container text-center" style="justify-content: center;">
        <button class="navbar-brand" data-bs-toggle="tooltip" data-bs-placement="top" title="My LinkedIn" onclick="window.open('https://www.linkedin.com/in/komal-chamyal-18248b1b3/','_blank')">
          <img src="linkedin.png" alt="" width="25" height="25" class="d-inline-block rounded align-text-top">
        </button>
        <button class="navbar-brand" onclick="window.open('https://github.com/komalchamyal','_blank')" data-bs-toggle="tooltip" data-bs-placement="top" title="My GitHub" target="_blank">
          <img src="github.png" alt="" width="25" height="25" class="d-inline-block rounded align-text-top">
        </button>
        <button class="navbar-brand" onclick="window.open('mailto:komalchamyal22@gmail.com','_blank')" data-bs-toggle="tooltip" data-bs-placement="top" title="Compose Mail" target="_blank">
          <img src="mail.png" alt="" width="25" height="25" class="d-inline-block rounded align-text-top">
        </button>
      </div>
    </nav>
  </div>

</template>

<script>
export default {
  name: 'first-page',
  props: {
    msg: String
  }
}
</script>


<style scoped>
.navbar-brand{
  opacity: 0.7;
  background-color: transparent;
  border: 0;
  margin: 0 2px;
  padding-bottom: 0;
  /* padding-top: 0; */
}
.navbar-brand:hover, .navbar-brand:active{
  opacity: 1;
}

/* image zoom */
.myimg {
  animation-delay: 1800ms;
  height: 42vh;
  max-height: 1440px;
  transform: scale(0.90);
  transition: transform .2s;
  border-radius: 200px;
}

.myimg:hover {
  transform: scale(1);
}

/* Typing intro */
.wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  place-items: center;
  height: 100vh;
  justify-content: space-evenly;
}

.typing-text {
  width: 23ch;
  animation: typing 3s steps(20), blink 0.5s step-end infinite alternate;
  white-space: nowrap;
  border-right: 2px solid;
  overflow: hidden;
  font-family: monospace;
  font-size: 2em;
  margin-top: 0.5ch;
  min-height: 3ch;
  margin-bottom: 0.5ch;
}

@keyframes typing {
  from {
    width: 0
  }
}

@keyframes blink {
  50% {
    border-color: transparent
  }
}

/* buttons */

.buttons {
  animation-delay: 3.3s;
  margin-bottom: 20vh;
  display: flex;
  flex-wrap: wrap;
  width: 85%;
  align-items: center;
  justify-content: space-evenly;
}

.button-28 {
  margin-top: 1ch;
  appearance: none;
  background-color: transparent;
  border: 2px solid black;
  border-radius: 15px;
  box-sizing: border-box;
  color: #000000;
  cursor: pointer;
  display: inline-block;
  font-family: Roobert, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 100%;
  font-weight: 600;
  line-height: normal;
  min-height: 40px;
  min-width: 100px;
  outline: none;
  margin: 5px 5px;
  text-align: center;
  text-decoration: none;
  transition: all 600ms cubic-bezier(.23, 1, 0.32, 1);
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  width: 14%;
  will-change: transform;
}

.button-28:hover {
  color: #fff;
  background-color: black;
  box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
  transform: translateY(-2px);
}

.button-28:active {
  box-shadow: none;
  transform: translateY(0);
}


@media only screen and (max-width: 768px) {
  .button-28 {
    width: 40%;
    font-size: small;
  }
}

@media only screen and (max-width: 500px) {

  /* For mobile phones: */
.buttons {
  margin-bottom: 25vh;
}
  .button-28 {
    width: 70%;
  }

  .typing-text {
    font-size: 1.5rem;
  }

}


/* @media (max-width: 354px){

  .typing-text {
    padding: 0 5ch;
  width: 14ch;
  animation: typing 2s steps(14), blink 0.3s step-end infinite alternate;
  white-space: nowrap;
  border-right: 2px solid;
  overflow: hidden;
  font-family: monospace;
  font-size: 2px;
  margin-top: 0.5ch;
  //min-height: 2ch;
  margin-bottom: 0.5ch;
}

} */
</style>
