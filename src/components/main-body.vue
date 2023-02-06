<template>
  <v-main class="main-body" id="main-body">
    <section class="intro-section" id="home">
      <v-row class="align-center px-10" style="height: 690px">
        <v-col lg="6" cols="6" class="pa-6 font-width-bold py-16">
          <h2 class="display-3">
            Full <span style="color: #2c97d3">Stack</span> &
            <span style="color: #d3682c">Front-End </span>Developer
          </h2>
          <v-subheader>
            <br />
            <br />
            Hey, <br />
            I'm Rahul, focusing on creating new things, and try to work on
            unique ideas.</v-subheader
          >
          <br />
          <br />
          <a
            href="mailto: rahulbanik98@gmail.com"
            style="text-decoration: none"
          >
            <v-btn
              large
              elevation="5"
              class="white--text mt-10 px-10 py-5"
              color="#2c97d3"
              >Hire Me</v-btn
            >
          </a>

          <a href="#contact-us" style="text-decoration: none">
            <v-btn
              large
              elevation="5"
              class="white--text mt-10 px-10 ml-10 py-5"
              color="#d3682c"
              >Contact</v-btn
            ></a
          >
          <v-row class="mt-16">
            <!-- chip section -->
            <chipSection></chipSection>
          </v-row>
        </v-col>
        <v-col>
          <v-img src="../image/Rahul Banik.jpg" class="image-section"></v-img>
        </v-col>
      </v-row>
    </section>
    <aboutSection />

    <educationSection />
    <br />
    <experienceSection />
    <br />
    <projectSection />
    <br />
    <contactusSection />
  </v-main>
</template>

<script>
import chipSection from "./smallComponents/chip-section.vue";
import aboutSection from "./about-section.vue";
import educationSection from "./education-section.vue";
import experienceSection from "./experience-section.vue";
import projectSection from "./projects-section.vue";
import contactusSection from "./contactus-section.vue";

export default {
  name: "main-body",
  components: {
    chipSection,
    aboutSection,
    educationSection,
    experienceSection,
    projectSection,
    contactusSection,
  },
};
</script>

<style>
html {
  scroll-behavior: smooth;
}
.main-body {
  background-color: #dce2e0;
  background-image: linear-gradient( hsl(320, 33%, 98%),#e4f7e770);
}
.image-section {
  margin-left: 30%;
  height: 50%;
  width: 50%;
}
</style>