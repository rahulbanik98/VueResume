<template>
  <section class="contact-us pt-10" id="contact-us">
    <v-img
      class="pt-10"
      gradient="to bottom, rgb(166 199 156), rgb(227 227 227 / 86%)"
      src="https://img.freepik.com/free-photo/contact-us_36325-2135.jpg?size=626&ext=jpg"
    >
      <v-container>
        <h4 class="display-1 text-center mb-5">
          I’m a developer, based in Kolkata. Currently a front-end developer.
          You can see my activities on
          <strong> Rahul Banik (Linkedin) </strong>profile.
        </h4>
        <v-divider />
        <br />
        <v-row>
          <v-col cols="12" lg="6">
            <v-card-title>DROP A LINE</v-card-title>
            <v-form action="https://formspree.io/f/xwkzgndz" method="POST">
              <v-text-field label="Your Name" id="name" name="name"/>
              <v-text-field label="Email" id="email" name="email"/>
              <v-text-field label="Subject" id="subject" name="subject"/>
              <v-textarea label="Message" id="message" name="message"/>
              <v-btn type="submit" large color="#d3682c" class="white--text"
                >Send Message</v-btn
              >
            </v-form>
          </v-col>
          <v-col cols="12" lg="3" offset="2">
            <v-card-title><h1>CONTACT ME</h1></v-card-title>
            <v-card-text>
              <h3 style="margin-bottom: 10px">
                <a href="https://goo.gl/maps/NYqCisZL82zkGEWR7">
                  66/2/3 'K' Road Howrah, 711108</a
                >
              </h3>

              <h3 style="margin-bottom: 10px">+91 8013240357</h3>

              <h3 style="margin-bottom: 10px">rahulbanik98@gmail.com</h3>
            </v-card-text>
            <v-card-actions>
              <a
                href="https://drive.google.com/file/d/14xAsSWuXWiG6AZzDdoJgvqBSFSgLcAfv/view"
                style="text-decoration: none"
                target="_blank"
              >
                <v-btn
                  large
                  elevation="5"
                  color="#2c97d3"
                  class="white--text mt-10 px-10 py-5"
                  >Download Resume
                  <v-icon>mdi-download</v-icon>
                </v-btn>
              </a>
            </v-card-actions>
          </v-col>
        </v-row>
      </v-container>
      <v-footer class="mt-4">
        <v-col class="text-center" cols="12">
          <strong>
            Copyright @{{ new Date().getFullYear() }} All rights Reserved | This
            is made by
            <a
              href="https://www.linkedin.com/in/rahul-banik-8b06aab0/"
              class="green--text"
              >Rahul Banik</a
            >
          </strong>
        </v-col>
      </v-footer>
    </v-img>
  </section>
</template>

<script>
export default {
  name: "contactus-section",
};
</script>

<style>
</style>