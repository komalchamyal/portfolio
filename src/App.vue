<template>
  <gotop></gotop>
  <Main></Main>
  <About></About>
  <Projects></Projects>
  <Skills></Skills>
  <Contact></Contact>
</template>

<script>
import Main from './components/Main.vue';
import gotop from './components/gotop.vue';
import About from './components/about.vue';
import Projects from './components/projects.vue';
import Skills from './components/skills.vue';
import Contact from './components/contact.vue';

export default {
  name: 'App',
  components: {
    Main, About, Projects, Skills, Contact,gotop,
    
},
  data() {
    return {
    }
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');

.heading{
  font-family: 'Montserrat', sans-serif;
  display: inline-block;
  position: relative;
  color: #3E2723;
  font-weight: 400;
  border-bottom: #3E2723 2px solid;
}

.heading::after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  left: 0;
  background-color: #6e5d5d;
  transition: transform 0.25s ease-out;
}

.heading:hover::after {
  transform: scaleX(1);
}

.subheading{
  font-family: 'Montserrat', sans-serif;;
 display: inline-block;
  position: relative;
  color: #3E2723;
  font-weight: 400;
}

.subheading::after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 1px;
  bottom:0;
  left: 0;
  background-color: #9e8686;
  transition: transform 0.25s ease-out;
}

.subheading:hover::after {
  transform: scaleX(1);
}
</style>
