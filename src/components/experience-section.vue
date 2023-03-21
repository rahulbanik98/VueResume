<template>
  <section class="experience" id="experience">
    <v-img height="500" src="https://designshack.net/wp-content/uploads/Home-office.jpg"
      gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)">
      <v-container>
        <h4 class="display-2 text-center"
          style="font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;">
          Experience</h4>
        <v-timeline>
          <v-timeline-item v-for="(exper, index) in experience" :key="index"
            :color="index % 2 === 0 ? '#d3682c' : '#2c97d3'">
            <v-card class="rounded-xl">
              <v-card-title>{{ exper.title }}</v-card-title>
              <v-card-text>
                {{ exper.date }}<br />
                @{{ exper.company }} <br />
                {{ exper.decription }}
              </v-card-text>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </v-container>
    </v-img>
  </section>
</template>

<script>
export default {
  name: "experience-section",
  data: () => ({
    experience: [
      {
        title: "VueJs Developer",
        date: "6 Month",
        company: " Global Ids",
        decription: "Work on HTML, CSS, Javascript, VueJs and Vetify",
      },
      {
        title: "ReactJs Developer",
        date: "1 Month",
        company: " RedoQ Ltd",
        decription: "Work on HTML, CSS, Javascript, ReactJs, Redux",
      },
      {
        title: "Frontend Developer",
        date: "2 Month",
        company: " Sk Private Ltd",
        decription: "Work on HTML, CSS, Javascript",
      },
    ],
  }),
};
</script>

<style></style>