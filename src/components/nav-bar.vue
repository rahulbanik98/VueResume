<template>
  <v-app-bar app elevation="0">
    <v-subheader
      ><h1 style="color: #2c97d3">My</h1>
      <br />
      <h3 style="color: #d3682c">Portfolio</h3></v-subheader
    >
    <v-tabs
      center-active
      right
      background-color="transparent"
      active-class="active-tab"
    >
      <v-tab
        ><a href="#main-body" style="text-decoration: none"> Home</a></v-tab
      >
      <v-tab><a href="#about-me" style="text-decoration: none">About</a></v-tab>
      <v-tab
        ><a href="#education-text" style="text-decoration: none"
          >Education</a
        ></v-tab
      >
      <v-tab
        ><a href="#experience" style="text-decoration: none"
          >Experience</a
        ></v-tab
      >
      <v-tab
        ><a href="#projects" style="text-decoration: none">Projects</a></v-tab
      >
    </v-tabs>
    <a href="mailto: rahulbanik98@gmail.com" style="text-decoration: none">
      <v-btn large color="#2c97d3" class="white--text ml-10"
        >Send me a Mail</v-btn
      ></a
    >
  </v-app-bar>
</template>

<script>
// import About from "./about-section.vue";

export default {
  name: "nav-bar",
  // components: About,
};
</script>

<style>
</style>