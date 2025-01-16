<script setup lang="ts">
import Profile from './components/Profile.vue';
import NavBar from "@/components/NavBar.vue";
import RightSection from "@/components/RightSection.vue";

</script>

<template>
  <header>
    <div class="wrapper">
      <NavBar name="Shah Fahad" profession="Software Engineer"/>
      <div class="content">
        <div class="left-cont">
          <Profile name="Shah Fahad" profession="Software Engineer"/>
        </div>
        <div class="right-cont">
          <RightSection/>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>

header {
  display: flex;
  place-items: center;
  line-height: 1.5;
  max-height: 100vh;
}

header .wrapper {
  display: flex;
  width: 100%;
  height: 100vh;
  flex-direction: column;
  place-items: flex-start;
  flex-wrap: wrap;
}

header > .wrapper > .content {
  display: flex;
  width: 100%;
  flex: 1;
}

header > .wrapper > .content > .left-cont {
  display: flex;
  flex: 1;
  width: 100%;
  background-color: #ff926e;
  position: relative;
}

header > .wrapper > .content > .right-cont {
  display: flex;
  flex-direction: column;
  justify-content: center;
  flex: 1;
  width: 100%;
  background-color: white;
  color: #282828;
  padding: 0 5rem;
}


</style>
