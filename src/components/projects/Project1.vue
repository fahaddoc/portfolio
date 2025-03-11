<script setup lang="ts">

defineProps<{
  imageLeft: string,
  imageRight: string,
  description: string
}>();

</script>

<template>
  <div class="col">
    <div class="row">
      <div class="left-box">
        <div class="cont lft">
          <img alt="" :src="imageLeft" height="300"/>
          <div class="para">
            <p>Flutter app which run in various platforms, Flutter app which run in various platforms,
              Flutter app which run in various platforms,Flutter app which run in various platforms,Flutter app which run
              in various platforms,Flutter app which run in various
              platforms.
            </p>
          </div>
        </div>
      </div>
      <div class="right-box">
        <div class="cont rt">
          <img alt="" :src="imageRight" height="300"/>
          <div class="para">
            <p>Flutter app which run in various platforms, Flutter app which run in various platforms,
              Flutter app which run in various platforms,Flutter app which run in various platforms,Flutter app which run
              in various platforms,Flutter app which run in various
              platforms.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="description">
      {{ description }}
    </div>
  </div>
</template>

<style scoped>
.col {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.col > .row {
  display: flex;
  justify-content: center;
  width: 100%;
}

.row > .left-box {
  display: flex;
  justify-content: center;
  padding: 0.5rem 0;
  flex: 1;
  width: 100%;
  background-color: white;
}

.row > .right-box {
  display: flex;
  justify-content: center;
  flex: 1;
  width: 100%;
  background-color: #ff926e;
}

.cont{
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 80%;
  margin: 1rem;
}

.cont.lft{
  border: 1px solid black;
  border-radius: 1rem;
}

.cont.rt{
  border: 1px solid white;
  border-radius: 1rem;
}

.cont > img{
  border-radius: 1rem;
}
.cont > .para {
  display: flex;
  width: 100%;
  color: #222222;
  justify-content: center;
  margin: 1rem;
  padding: 0 0.5rem;
}


</style>