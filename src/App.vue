<script setup lang="ts">
import NavBar from './components/NavBar.vue';
import HomeView from './views/HomeView.vue';
import ProjectsView from './views/ProjectsView.vue';
import Contact from './views/ContactView.vue'

</script>

<template>
  <NavBar name="Shah Fahad" profession="Software Engineer"/>
  <HomeView/>
  <ProjectsView/>
  <Contact/>
</template>

<style>
section {
  display: flex;
  flex-direction: column;
  place-items: center;
  line-height: 1.5;
  max-height: 100vh;
  background-color: #2c3e50 !important;
}
</style>

