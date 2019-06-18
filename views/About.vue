<template>
  <v-container fluid class="about">
    <v-layout column>
      <v-flex xs6 md6 mt-10 align-self-center>
        <v-card xs4 color="#242526" dark class="about-card border">
          <v-img :src="require('../assets/rolls.jpg')" contain />"
          <v-card-text class="headline text-xs-center text-uppercase">
            The first and most established of Merced's Sushi restaurants.
            <hr />
          </v-card-text>
          <v-card-text class="subheading mt-2 text-xs-center">
            King's Asian Cuisine provides its customers with friendly service,
            great food, and a positive atmosphere. We welcome families and
            individuals of all ages as we have something for anybody in the
            group. We serve both Chinese and Japanese Cuisine ranging from fried
            rice to sushi rolls and sashimi.
          </v-card-text>
          <v-card-actions>
            <v-btn flat dark color="white" to="/">Back To Home</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "About",
  components: {}
};
</script>

<style>
.about {
  background: url("../assets/swirl.jpg");
  height: 100%;
  width: 100%;
}
.about-card {
  width: 500px;
}
</style>
