<template>
  <v-container fluid fill-height class="about">
    <v-layout column>
      <v-layout row wrap mt-5 fill-height align-self-center>
        <v-flex mb-5 id="about-grid" align-self-center>
          <v-card xs4 color="#242526" dark class="about-card border">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3173.768957901207!2d-120.48397428442479!3d37.30060924706988!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80914301ff8b32f7%3A0xa81f32077d2eee23!2s360+W+Main+St%2C+Merced%2C+CA+95340!5e0!3m2!1sen!2sus!4v1561626248891!5m2!1sen!2sus"
              width="500"
              height="300"
              frameborder="0"
              style="border:0"
              allowfullscreen
            ></iframe>
            <v-card-text class="headline text-xs-center text-uppercase">
              Location and Hours
              <hr />
            </v-card-text>
            <v-card-text class="subheading mt-2 text-xs-center">
              360 W Main St. <br />
              Merced, CA 95340<br />
              <a class="link" href="tel:2093839838">(209) 383-9838</a>
              <br />
              <br />
              <strong>Business Hours:</strong><br />
              Tuesday-Thursday: 11am to 9pm<br />
              Friday: 11am to 10pm<br />
              Saturday: 12pm to 10pm<br />
              Sunday: 12pm to 9pm
            </v-card-text>
            <v-card-actions>
              <v-btn flat dark color="white" to="/">Back To Home</v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>
      </v-layout>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "location"
};
</script>

<style scoped>
.about {
  background: url("../assets/swirl.jpg");
  height: 100%;
  width: 100%;
}
</style>
