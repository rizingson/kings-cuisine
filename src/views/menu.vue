<template>
  <v-container fluid class="menu-page">
    <v-layout row xs12 wrap>
      <v-flex xs9 md4 class="pa-3">
        <v-img :src="require('../assets/menu1.jpg')" class="border" />
      </v-flex>
      <v-flex xs9 md4 class="pa-3">
        <v-img :src="require('../assets/menu2.jpg')" class="border" />
      </v-flex>
      <v-flex xs9 md4 class="pa-3">
        <v-img :src="require('../assets/menu3.jpg')" class="border" />
      </v-flex>
      <v-flex xs9 md4 class="pa-3">
        <v-img :src="require('../assets/menu4.jpg')" class="border" />
      </v-flex>
      <v-flex xs9 md4 class="pa-3">
        <v-img :src="require('../assets/menu5.jpg')" class="border" />
      </v-flex>
      <v-flex class=" home-button pa-3" align-baseline>
        <v-card color="#242526" dark>
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
  name: "menu",
  components: {}
};
</script>

<style scoped>
.menu-page {
  height: 100%;
  width: 100%;
  padding: 0%;
  background: url("../assets/swirl.jpg");
}
.home-button {
  width: auto;
  position: fixed;
}
</style>
