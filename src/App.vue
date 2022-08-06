<template>
  <div>
    <MainPage />
  </div>
</template>

<script>
import "@/assets/styles/reset.css";
import "@/assets/styles/global.css";

import MainPage from "./components/MainPage.vue";

export default {
  name: "App",
  components: {
    MainPage
},
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&display=swap");
</style>
