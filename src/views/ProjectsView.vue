<script setup lang="ts">
import Project1 from '@/components/projects/Project1.vue';
import imageLeft from '@/assets/projects/project1/digitalhire_1.png';
import imageRight from '@/assets/projects/project1/digitalhire_2.webp';
</script>

<template>
  <div class="heading">
    <span>My Work</span>
  </div>
  <Project1
      :imageRight="imageRight"
      :imageLeft="imageLeft"
      leftDescription="Flutter app which run in various platforms, Flutter app which run in various platforms,
              Flutter app which run in various platforms,Flutter app which run in various platforms,Flutter app which run
              in various platforms,Flutter app which run in various
              platforms."
      rightDescription="Flutter app which run in various platforms, Flutter app which run in various platforms,
              Flutter app which run in various platforms,Flutter app which run in various platforms,Flutter app which run
              in various platforms,Flutter app which run in various
              platforms."
  />
</template>

<style scoped>
.heading {
  display: flex;
  width: 100%;
  justify-content: center;
  justify-items: center;
  background-color: #2c3e50;
  padding: 0.5rem 0;
}

.heading span {
  color: #dad7d3;
  font-size: 32px;
  font-weight: bolder;
  border-bottom: #eb4813 2px solid;
}

</style>
