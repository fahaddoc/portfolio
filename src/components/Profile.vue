<script setup lang="ts">
defineProps<{
  name: string
  profession: string
}>()
</script>

<template>
  <div class="profile-card">
    <div class="profile-image">
      <img src="@/assets/profile_image.jpg"/>
      <h1 class="profile-name">{{name}}</h1>
      <span class="profession">{{profession}}</span>
    </div>
    <div class="profile-card-footer">
      <img src="@/assets/fb.webp"/>
      <img src="@/assets/xtwitter.webp"/>
      <img src="@/assets/linkedIn.webp"/>
      <img src="@/assets/insta.webp"/>
    </div>
  </div>
</template>

<style scoped>

.profile-card{
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 3rem;
  right: -3rem;
  background-color: #dad7d3;
  color: #282828;
  width: 375px;
  height: 526px;
  box-shadow: -11px 20px 40px 0 rgba(0,0,0,0.6);
}

.profile-card > .profile-image{
  display: flex;
  flex-direction: column;
  flex: 1;
  align-items: center;
  justify-content: center;
  border: transparent;
  border-radius: 50%;
}

.profile-card > .profile-image > img{
  width: 205px;
  height: 205px;
  border-radius: 50%;
  background-repeat: no-repeat;
}

.profile-card > .profile-image > .profile-name{
  margin: 2rem 0;
  border-bottom: #eb4813 2px solid;
}

.profile-card > .profile-image > .profession{
  font-family: "sans-serif";
  letter-spacing: 0.25em;
}

.profile-card > .profile-card-footer{
  display: flex;
  justify-content: center;
  background-color: white;
  padding: 14px 0;
  gap: 18px;
}

.profile-card > .profile-card-footer > img{
  width: 25px;
  height: 25px;
}


</style>
