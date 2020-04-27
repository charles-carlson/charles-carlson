<template>
  <div id="app">
    <Header/>
    <About/>
    <Skills/>
    <Experience/>
    <Projects/>
    <Interests/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Experience from './components/blocks/Experience.vue'
import Interests from './components/blocks/Interests.vue'
import Projects from './components/blocks/Projects.vue'
import Skills from './components/blocks/Skills.vue'
import About from './components/blocks/About.vue'
export default {
  name: 'App',
  components: {
    Header,
    Experience,
    Interests,
    Projects,
    Skills,
    About
  }
}
</script>

<style>
  div{
    background-color: #1e1e1e;
    overflow: hidden;
  }
</style>
