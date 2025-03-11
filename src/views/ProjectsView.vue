<script setup lang="ts">
import Project1 from '@/components/projects/Project1.vue';
import imageLeft from '@/assets/projects/project1/digitalhire_1.png';
import imageRight from '@/assets/projects/project1/digitalhire_2.webp';
</script>

<template>
    <div class="heading">
        My Work
    </div>
    <Project1 :imageRight="imageRight" :imageLeft="imageLeft" description="shhs"/>
</template>

<style scoped>
.heading{
  display: flex;
  width: 100%;
  justify-content: center;
  justify-items: center;
  font-size: 32px;
  background-color: gray;
}
</style>
