<script setup lang="ts">
import Profile from '@/components/Profile.vue';
import RightSection from '@/components/RightSection.vue';

</script>

<template>
  <section>
    <div class="wrapper">
      <div class="content">
        <div class="left-cont">
          <Profile name="Shah Fahad" profession="Software Engineer"/>
        </div>
        <div class="right-cont">
          <RightSection/>
        </div>
      </div>
    </div>
  </section>
</template>

<style>

section .wrapper {
  display: flex;
  width: 100%;
  height: 100vh;
  flex-direction: column;
  place-items: flex-start;
  flex-wrap: wrap;
}

section > .wrapper > .content {
  display: flex;
  width: 100%;
  flex: 1;
}

section > .wrapper > .content > .left-cont {
  display: flex;
  flex: 1;
  width: 100%;
  background-color: #ff926e;
  position: relative;
}

section > .wrapper > .content > .right-cont {
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
