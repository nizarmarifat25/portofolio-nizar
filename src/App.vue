<template>
  <NavbarComp />
  <Hero />
  <About />
  <Experience />
  <Project />
  <Footer />
</template>

<script>
import NavbarComp from './components/NavbarComp.vue';
import Hero from './components/Hero.vue';
import About from './components/About.vue';
import Experience from './components/Experience.vue';
import Project from './components/Project.vue';
import Footer from './components/Footer.vue';
export default {
  name: 'App',
  components: {
    NavbarComp,
    Hero,
    About,
    Experience,
    Project,
    Footer
  }
}
</script>

<style>
body {
  color: white;
  font-family: 'Montserrat', sans-serif;
  background: #003049 !important;
  overflow-x: hidden;
}

.title {
  color: #ffc300;
}
</style>
