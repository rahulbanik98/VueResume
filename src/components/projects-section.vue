<template>
  <section class="portfolio">
    <h4 class="display-2 text-center">Projects</h4>
    <br />
    <v-slide-group class="pa-4" active-class="success">
      <v-slide-item
        class="slideSections"
        v-for="(slider, index) in projectTitle"
        :key="index"
      >
        <v-card
          height="250"
          width="250"
          class="cardClass mx-2"
          style="text-align: center"
        >
          <div class="sliderName">
            <h4>{{ slider.name }}</h4>
          </div>
          <div class="sliderBody">
            <v-card-text>{{ slider.body }}</v-card-text>
          </div>
          <div>
            <h5>Date: {{ slider.date }}</h5>
          </div>
        </v-card>
      </v-slide-item>
    </v-slide-group>
  </section>
</template>

<script>
export default {
  name: "projects-section",
  data: () => ({
    model: null,
    projectTitle: [
      {
        name: "Created a Navigation Bar",
        body: " created a new navbar component for the updated version. I use VueJs, Vuetify, VueJs router, and Javascript for this component.",
        date: "09/2022 - 09/2022",
      },
      {
        name: "Add a skeleton loader",
        body: "Add skeleton loader component and add on the table pages",
        date: "12/2022 - 12/2022",
      },
      {
        name: "JSON viewer for JSON data user",
        body: "Create a JSON data viewer for JSON users",
        date: "09/2022 - 09/2022"
      },
      {
        name: "Created a Business Website",
        body: "his project helped to switch businesses online. For this project, I use HTML, CSS, and JavaScript. In the future, I include some other technologies.",
        date: "05/2022 - 06/2022",
      },
      {
        name: "Portfolio Website",
        body: "The website created by Vuejs and Vuetify, In this website each and every component is reusebale component. This Website shows each and every detels of the person.",
      },
      { name: "OTP Based Login System", body: "Body1" },
      { name: "ShareBit", body: "Body2" },
      { name: "Phonenumber Validator", body: "Body3" },
    ],
  }),
};
</script>

<style>
.cardClass {
  background-image: conic-gradient(#dedcf5b4, #dcf5e2b7, #f1d6d1ce);
  border-width: 1px;
  border-style: solid;
  border-image: linear-gradient(#769df3, #fdaca1f3) 1 1%;
}

.sliderName {
  margin-top: 10%;
  height: 10%;
  width: 100%;
}
</style>