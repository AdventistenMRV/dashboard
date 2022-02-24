<script setup lang="ts">
// import TheWelcome from "@/components/TheWelcome.vue";
</script>

<template>
  <div class="background"></div>
  <div class="sevenGridContainer">
    <div class="appView">
      <div class="centerElement">
        <div class="title">
          <div></div>
          <img
            class="icon"
            src="@/assets/images/adventist-symbol-circle--white.svg"
          />
          <div class="text">dashboard.mrv.adventisten.de</div>
          <div></div>
        </div>
        <div class="appGrid"></div>
      </div>
    </div>
    <div class="seventhGrid"></div>
  </div>
</template>

<style scoped>
.background {
  background-image: url("@/assets/images/background.jpg");
  height: 100vh;
  width: 100vw;
  background-size: cover;
  background-repeat: no-repeat;
  filter: blur(4px);
  z-index: 1;
  opacity: 0.8;
}
.sevenGridContainer {
  width: 100%;
  height: 100%;
  display: grid;
  grid-auto-columns: 1fr;
  grid-template-columns: 6fr 1fr;
  grid-template-rows: 1fr;
  gap: 0px 0px;
  grid-template-areas: ". .";

  z-index: 2;
}

.centerElement {
  width: 75%;
  height: 500px;
  -webkit-animation: expand 5s;
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}
.title {
  text-align: center;
  vertical-align: middle;
  color: #ffffff;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  font-size: 2em;

  display: grid;
  grid-auto-columns: 1fr;
  grid-template-columns: auto min-content min-content auto;
  grid-template-rows: 1fr;
  gap: 0px 0px;
  grid-template-areas: ". . . .";
  margin-bottom: 1em;
}

.icon {
  height: 3em;
}

.text {
  font-size: 1.2em;
  padding-top: 0.65em;
  padding-left: 0.5em;
}
</style>
