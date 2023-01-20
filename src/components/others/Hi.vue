<template>
    <h1 class="ml8 text-center">
  <span class="letters-container">
    <span class="letters letters-left">Hi</span>
    <span class="letters bang">!</span>
  </span>
  <span class="circle circle-dark"></span>
  <span class="circle circle-container"><span class="circle circle-dark-dashed"></span></span>
</h1>
</template>

<script>
import anime from 'animejs/lib/anime.es.js';
export default {
  name: 'Hi-intro',
  methods: {
    animateText() {
      anime.timeline({ loop: true })
        .add({
          targets: '.ml8 .circle-container',
          scale: [0, 1],
          duration: 1100,
          easing: "easeInOutExpo",
          offset: '-=1000'
        }).add({
          targets: '.ml8 .circle-dark',
          scale: [0, 1],
          duration: 1100,
          easing: "easeOutExpo",
          offset: '-=600'
        }).add({
          targets: '.ml8 .letters-left',
          scale: [0, 1],
        }).add({
          targets: '.ml8 .bang',
          scale: [0, 1],
          rotateZ: [45, 15],
          duration: 700,
          //offset: '-=200'
        }).add({
          targets: '.ml8',
          opacity: 0,
          duration: 1000,
          easing: "easeOutExpo",
          delay: 1000
        });

      anime({
        targets: '.ml8 .circle-dark-dashed',
        rotateZ: 360,
        duration: 8000,
        easing: "linear",
        loop: true
      });


      // targets: '.letter',
      // opacity: 1,
      // //translateX: 150, 
      // delay: anime.stagger(100, {start: 1000}), 
      // //translateX: [0, 30]
      // // targets: '.anim',
      // // translateX: 270,
      // // easing: "linear",
      // // delay: anime.stagger(100)
    }
  },
  mounted() {
    this.animateText()
  },
}
</script>

<style scoped>

h1.ml8 {
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  top: 0;
  bottom: 0;
  font-weight: 900;
  font-size: 4.5em;
  color: rgb(255, 255, 255);
  width: 3em;
  height: 3em;
}

.ml8 .letters-container {
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  top: 0;
  bottom: 0;
  height: 1em;
}

.ml8 .letters {
  position: relative;
  z-index: 2;
  display: inline-block;
  line-height: 0.7em;
  right: -0.12em;
  top: -0.2em;
  left: -0.001em;
}

.ml8 .bang {
  font-size: 1.4em;
  top: auto;
  /* left: -0.08em; */
}

.ml8 .circle {
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  top: 0;
  bottom: 0;
}

.ml8 .circle-dark {
  width: 2.2em;
  height: 2.2em;
  background-color: #393939;
  border-radius: 3em;
  z-index: 1;
}

.ml8 .circle-dark-dashed {
  border-radius: 2.4em;
  background-color: transparent;
  border: 2px dashed #ffffff;
  width: 2.3em;
  height: 2.3em;
}
</style>