<script setup lang="ts">
defineProps<{
  name: string,
  profession: string,
}>()
</script>

<template>
  <div class="header">
    <div class="left">
      <div class="profile-name-holder">
        <span class="sq-box"></span>
        <div class="name">{{name}}</div>
      </div>
      <div class="profession">{{profession}}</div>
    </div>
    <div class="right">
      <div class="nav">
        <div class="li on">About Me</div>
        <div class="li">Resume</div>
        <div class="li">Products / Projects</div>
        <div class="li">Contact</div>
      </div>
    </div>
  </div>
</template>

<style>

.header{
  display: flex;
  background-color: #2c3e50;
  width: 100%;
  padding: 24px;
}

.header .left{
  display: flex;
  align-items: center;
  flex: 1;
}

.header .left > .profile-name-holder{
  display: flex;
  align-items: center;
}

.header .left > .profile-name-holder > .sq-box{
  display: flex;
  width: 16px;
  height: 16px;
  margin-right: 0.5rem;
  background-color: #eb4813;
}

.header .left > .profile-name-holder > .name{
  display: flex;
}

.header .profession{
  font-family: "sans-serif";
  letter-spacing: 0.25em;
  margin: 0 1rem;
}

.header .right{
  display: flex;
  justify-content: flex-end;
  flex: 1;
}

.header .right > .nav{
  display: flex;
  align-items: center;
  gap: 1rem;
}

.header .right > .nav > .li{
  cursor: pointer;
  text-transform: capitalize;
  font-size: 16px;
}

.header .right > .nav > .li.on{
  color: white;
}

.header .right > .nav > .li:hover{
  color: white;
}



</style>