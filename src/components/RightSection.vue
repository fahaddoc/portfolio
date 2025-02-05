<script setup lang="ts">
import {ref, onMounted, type Ref} from 'vue';

const subGreetingText = ref<HTMLDivElement | null>(null);
let counter = -1;
let textArray: string[] = [];


const typeJs = (text: Ref<HTMLDivElement | null>) => {
  if(!text.value) return;
  const dataText = text.value.dataset.typetext ?? "";

  if(counter < dataText.length){
    counter++;
    text.value.innerHTML += dataText.charAt(counter);
    textArray = dataText.split(""); 
  }

}

onMounted(()=>{
  if(subGreetingText.value){
    subGreetingText.value.innerHTML = '';
    textArray = subGreetingText.value.dataset.typetext?.split('') ?? [];
    setInterval(()=> typeJs(subGreetingText),100);
  }
});

</script>

<template>
  <div class="greeting-text">Hi,</div>
  <div ref="subGreetingText" class="sub-greeting-text" data-typetext="Dynamic and versatile Software Engineer specializing in web and mobile application development. With a strong foundation in HTML, CSS, JavaScript, React, Node.js, and MongoDB, I create responsive, user-focused web solutions that engage and perform.
Recently, I’ve expanded my expertise to include Flutter for cross-platform mobile development and Next.js to deliver enhanced web performance. My experience with Python bots adds another dimension to my technical repertoire, showcasing my adaptability to diverse programming challenges.
Known for being a quick learner with excellent written and verbal communication skills, I thrive in fast-paced environments, managing multiple projects simultaneously while consistently meeting deadlines. Passionate about continuous learning, I embrace new challenges and stay updated with emerging technologies to deliver innovative solutions in the ever-evolving tech industry."></div>
<div class="actions">
    <button class="btn primary">Resume</button>
    <button class="btn secondary">Projects</button>
  </div>
</template>

<style>
.greeting-text {
  font-size: 100px;
  line-height: 1.2em;
}

.sub-greeting-text {
  font-size: 14px;
}

.actions{
  display: flex;
  width: 100%;
  gap: 8px;
  padding: 16px 0;
}

.actions > .btn{
  border: none;
  border-radius: 4px;
  padding: 12px;
  width: 200px;
  text-transform: capitalize;
  cursor: pointer;
}

.actions > .btn:hover{
  background-color: #efeaea !important;
  border: 1px solid #ff926e !important;
  color: #ff926e !important;
}

.actions > .btn.primary{
  background-color: #ff926e;
  color: white;
}

.actions > .btn.secondary{
  background-color: #fcfcfc;
  border: 1px solid #ff926e;
  color: #ff926e;
}

</style>