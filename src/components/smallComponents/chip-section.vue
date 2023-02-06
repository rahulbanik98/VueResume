<template>
  <div class="text-center">
    <a
      href="https://www.linkedin.com/in/rahul-banik-8b06aab0/"
      target="_blank"
      style="text-decoration: none"
    >
      <v-chip class="px-4 ma-3" color="info" style="cursor: pointer">
        <v-icon class="mr-2">mdi-linkedin </v-icon> Linkedin
      </v-chip>
    </a>

    <a
      href="https://github.com/rahulbanik98"
      target="_blank"
      style="text-decoration: none"
    >
      <v-chip class="ma-2" color="secondary" style="cursor: pointer"
        ><v-icon class="mr-2">mdi-github</v-icon> Github
      </v-chip>
    </a>

    <a
      href="https://www.facebook.com/rahul.banik.9469/"
      target="_blank"
      style="text-decoration: none"
    >
      <v-chip class="px-4 ma-3" color="primary" style="cursor: pointer"
        ><v-icon left size="20" class="mr-2">mdi-facebook</v-icon
        >Facebook</v-chip
      >
    </a>

    <a
      href="https://www.instagram.com/rahulbanik5/"
      target="_blank"
      style="text-decoration: none"
    >
      <v-chip
        class="ma-2"
        color="red"
        text-color="white"
        style="cursor: pointer"
        ><v-icon class="mr-2">mdi-instagram</v-icon> Instagram
      </v-chip>
    </a>
  </div>
</template>

<script>
export default {
  name: "chip-section",
};
</script>

<style>
</style>