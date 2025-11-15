<template>
  <div id="contact" class="text-center">
    <h1 class="heading display-3 pt-5">Get In Touch</h1>
    <br>
    <h2 class="fs-2 subheading">Leave me a Message!</h2>
    <div class="text-center">
      <p class="fs-6 lead px-5 mb-5">(Could be anything from `Hii Komal` to `I would like to work with you`)</p>
    </div>
    <div class="errors text-center space">
      <p class="error1 animate__animated">
        I actually get these messages you know
        <button type="button" class="close-1" aria-label="Close"><i class="bi bi-x-lg"></i></button>
      </p>
      <p class="error2 animate__animated">
        Would Love to know your name! (Even if it's a fake one)
        <button type="button" class="close-2" aria-label="Close"><i class="bi bi-x-lg"></i></button>
      </p>
      <p class="error3 animate__animated">No content. Can't let you spam no no
        <button type="button" class="close-3" aria-label="Close"><i class="bi bi-x-lg"></i></button>
      </p>
    </div>
    <div id="contact-form">
      <input type="text" autocomplete="off" name="name" class="input-name2 mx-3" placeholder="Your Name"
        data-bs-toggle="tooltip" title="Your name" required />

      <button id="msg-btn" type="submit" class="button-msg mx-3">
        <i id="change-icon" class="bi bi-send-fill"></i>
      </button>
      <textarea name="message" autocomplete="off" required data-bs-toggle="tooltip" data-bs-placement="bottom"
        title="Any comments" class="comments form-control mt-3" :value=msg placeholder="Type Something Here"></textarea>
    </div>

    <div class="text-center mt-4">
      <div id="#" class="thanks fs-1 animate__animated animate__backInLeft"
        style="font-family: 'Montserrat', sans-serif; font-weight: 100;"> Thank You!</div>
    </div>
    <div class="text-center">
      <h2 class="fs-4 subheading mt-4">For Work/Enquiry</h2><br>
      <div class="text-center" style=" font-family: 'Poppins', sans-serif;">
        <p class="mb-4 pb-3" style="font-size: small;">Email: komalchamyal22@gmail.com <br> or <br>
          <a href="mailto:komalchamyal22@gmail.com" class="danx"> Mail Me</a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'contact-section',
  props: {
    msg: String,
    name: String
  }

}

</script>

<style>
.bi-check-lg {
  font-size: 3ch;
  margin: 0;
  padding: 0;
  color: green;
}

.bi-x {
  font-size: 3ch;
  margin: 0;
  padding: 0;
  color: rgb(150, 0, 0);
}

.lds-hourglass {
  display: inline-block;
}

.lds-hourglass:after {
  content: " ";
  display: block;
  border-radius: 50%;
  z-index: 1000;
  width: 0;
  height: 0;
  box-sizing: border-box;
  border: 12px solid rgb(0, 0, 0);
  border-color: rgb(0, 0, 0) transparent black transparent;
  animation: lds-hourglass 1.2s infinite;
}

@keyframes lds-hourglass {
  0% {
    transform: rotate(0);
    animation-timing-function: cubic-bezier(0.55, 0.055, 0.675, 0.19);
  }

  50% {
    transform: rotate(900deg);
    animation-timing-function: cubic-bezier(0.215, 0.61, 0.355, 1);
  }

  100% {
    transform: rotate(1800deg);
  }
}


#contact {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}


.button-msg {
  transform: translateY(5px);
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
  outline: none;
  padding: 0;
  text-align: center;
  text-decoration: none;
  transition: all 200ms cubic-bezier(.23, 1, 0.32, 1);
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  width: 10%;
  min-width: 50px;
  will-change: transform;
}

.button-msg:not(.no-hover):hover {
  color: #fff;
  background-color: black;
  box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
  transform: translateY(-2px);
}

.button-msg:active {
  box-shadow: none;
  transform: translateY(0);
}

.close-1,
.close-2,
.close-3 {
  background-color: transparent;
  border: none;
}

.close-1:hover,
.close-2:hover,
.close-3:hover {
  color: rgb(66, 66, 66);
}

.errors {
  align-self: center;
  margin: 0 5%;
  font-family: 'Poppins', sans-serif;
}

.space {
  height: 2ch;
  margin-bottom: 1.5ch;
}

.heading {
  width: 12ch;
  align-self: center;
}

.subheading {
  width: 20ch;
  align-self: center;
}

svg {
  font-weight: lighter;
}

.input-name2 {
  width: 25%;
  height: 40px;
  position: relative;
  padding-left: 2ch;
  border-radius: 5px;
  max-width: 250px;
  outline: none;
  border: none;
  box-shadow: rgb(80, 68, 68) 4px 4px 4px;
  justify-content: center;
}

.comments {
  margin-left: auto;
  margin-right: auto;
  width: 50%;
  max-width: 500px;
  padding: 1ch;
  height: 15vh;
  outline: none;
  resize: none;
  box-shadow: black 10px 8px 1px;

}

@media only screen and (max-width: 1100px) {

  .errors {
    margin-bottom: 40px;
  }

  .input-name2 {
    width: 40%;
  }

  .comments {
    margin-left: auto;
    margin-right: auto;
    width: 70%;
    max-width: 500px;
  }
}

@media only screen and (max-width: 576px) {

  .input-name2 {
    width: 50%;
    font-size: medium;
  }

  .comments {
    height: 17vh;
    width: 80%;
    font-size: medium;
  }

}</style>