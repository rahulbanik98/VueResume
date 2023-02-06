<template>
  <v-app id="inspire">
    <!-- nav-section -->
    <navBar></navBar>

    <!-- main body part -->
    <mainBody></mainBody>
  </v-app>
</template>


<script>
import navBar from "./components/nav-bar.vue";
import mainBody from "./components/main-body.vue";

export default {
  components: {
    navBar,
    mainBody,
  },
};
</script>

<style>
</style>