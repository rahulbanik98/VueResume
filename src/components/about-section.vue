<template >
  <section class="about-me" id="about-me">
    <v-img
      class="pa-10"
      height="400"
      gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
      src="https://designshack.net/wp-content/uploads/Home-office.jpg"
    >
      <v-row justify="center" class="align-center">
        <v-col lg="6" cols="6">
          <v-card
            class="text-center pa-7 rounded-lg"
            color="#e1e0e0c9"
            elevation="6"
          >
            <v-card-subtitle style="color: #d3682c"
              ><h1>About Myself</h1></v-card-subtitle
            >
            <h3 style="text-align: center">
              Hello, I'm Rahul Banik. I'm from West Bangal Howrah. <br />
              I complete my Diploma in APC Ray Polytechnic year of 2019 and
              complete my B.Tech From St.Thomas College of Engineering and
              Technology year of 2022. I have 1 year of experience in
              Development and worked on HTML, CSS, JS, ReactJs, and VueJs.
            </h3>
            <a
              href="https://drive.google.com/file/d/1dfik1ILrbn2SKW441whR5ZEZ3b9_mk8E/view?usp=sharing"
              download
              style="text-decoration: none"
              target="_blank"
            >
              <v-btn
                large
                color="#2c97d3"
                class="white--text mt-7 px-7 py-3"
                elevation="5"
              >
                <!-- <a href="../cv/Rahul Banik.pdf" download> -->
                Download Resume<v-icon> mdi-download</v-icon></v-btn
              >
            </a>
          </v-card>
        </v-col>
        <v-col lg="6" cols="6">
          <v-card class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
            <div class="py-1" v-for="(item, index) in items" :key="index">
              <label>{{ item.title }}</label>
              <v-progress-linear
                :color="item.color"
                height="7"
                :value="item.value"
              ></v-progress-linear>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-img>
  </section>
</template>

<script>
export default {
  name: "about-section",
  data: () => ({
    drawer: null,
    items: [
      { title: "HTML", value: 80, color: "#e34c26" },
      { title: "CSS", value: 80, color: "#264de4" },
      { title: "Javascript", value: 75, color: "#f0db4f" },
      { title: "ReactJs", value: 70, color: "#87CEEB" },
      { title: "Vuejs", value: 70, color: "#42b883" },
      { title: "Python", value: 60, color: "#565d69" },
      { title: "Java", value: 65, color: "#78116a" },
    ],
  }),
};
</script>

<style>
</style>