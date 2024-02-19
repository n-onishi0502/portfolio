<template>
  <v-app>
    <NavBar/>
    <AboutMe id="aboutMe"/>
    <Skills id="skills"/>
  </v-app>
</template>

<script>
  import NavBar from '../components/NavBar'
  import AboutMe from '../components/AboutMe'
  import Skills from '../components/Skills'

  export default {
    name: 'Home',

    components: {
      NavBar,
      AboutMe,
      Skills
    },
  }
</script>

<style>

  .bg {
    width: 100vw;
    height: 100vh;
    background-image: linear-gradient(0deg, #00dedc, #115d89, #080f1c);
    display:flex;
  }

</style>