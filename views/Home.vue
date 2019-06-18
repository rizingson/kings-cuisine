<template>
  <v-container fluid class="home-page">
    <v-layout column>
      <v-flex lg12>
        <div id="header">
          <v-img :src="require('../../public/kingsLogo.png')" class="logo" />
          <span id="address"
            ><strong
              >360 W Main St. <br />
              Merced, CA 95340<br />
              <a class="link" href="tel:209383983">(209) 383-9838</a></strong
            ></span
          >
        </div>
      </v-flex>
      <v-flex>
        <v-carousel hide-delimiters height="650" dark class="bg" xs12>
          <v-carousel-item
            v-for="(item, i) in items"
            :key="i"
            :src="item.src"
          ></v-carousel-item>
        </v-carousel>
      </v-flex>
      <v-layout row wrap mt-5 fill-height align-self-center>
        <v-flex xs8 id="about-grid" align-self-center>
          <v-card color="#242526" dark class="about-card border">
            <v-card-text class="headline mt-5 text-xs-center text-uppercase">
              The first and most established of Merced's Sushi restaurants.
              <hr />
            </v-card-text>
            <v-card-text class="subheading mt-2 text-xs-center">
              King's Asian Cuisine provides its customers with friendly service,
              great food, and a positive atmosphere. We welcome families and
              individuals of all ages as we have something for anybody in the
              group. We serve both Chinese and Japanese Cuisine ranging from
              fried rice to sushi rolls and sashimi.
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
      <v-layout row wrap mt-5>
        <v-flex pa-3 xs3 lg3 id="lucky">
          <v-img :src="require('../assets/lucky.jpg')" class="border" />
        </v-flex>
        <v-flex pa-3 xs3 lg3>
          <v-img :src="require('../assets/special.jpg')" class="border" />
        </v-flex>
        <v-flex pa-3 xs3 lg3>
          <v-img :src="require('../assets/sunburst.jpg')" class="border" />
        </v-flex>
        <v-flex pa-3 xs3 lg3>
          <v-img :src="require('../assets/cherryBalls.jpg')" class="border" />
        </v-flex>
      </v-layout>

      <v-layout row wrap mt-5 fill-height align-self-center>
        <v-flex mb-5 id="about-grid" align-self-center>
          <v-card xs4 color="#242526" dark class="about-card border">
            <v-img :src="require('../assets/storeFront.jpg')" contain />"
            <v-card-text class="headline text-xs-center text-uppercase">
              Come visit us in downtown Merced!
              <hr />
            </v-card-text>
            <v-card-text class="subheading mt-2 text-xs-center">
              <strong>Business Hours:</strong><br />
              Tuesday-Thursday: 11am to 9pm<br />
              Friday: 11am to 10pm<br />
              Saturday: 12pm to 10pm<br />
              Sunday: 12pm to 9pm
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-layout>
  </v-container>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home",
  data() {
    return {
      appTitle: "Kings Asian Cuisine",
      drawer: false,
      items: [
        {
          src: require("../assets/cover.jpg")
        },
        {
          src: require("../assets/tylerRoll.jpg")
        },
        {
          src: require("../assets/bar2.jpg")
        },
        {
          src: require("../assets/booth.jpg")
        },
        {
          src: require("../assets/bakedMussels.jpg")
        },
        {
          src: require("../assets/dynamiteKings.jpg")
        },
        {
          src: require("../assets/beefBento.jpg")
        }
      ]
    };
  }
};
</script>

<style>
#header {
  background-color: #242526;
  height: 136px;
  width: 100%;
  overflow: hidden;
  align-content: center;
}
.home-page {
  height: 100%;
  width: 100%;
  padding: 0%;
  background: url("../assets/swirl.jpg");
}
.about-card {
  width: 500px;
}
.logo {
  height: 140px;
  width: 165px;
}
span {
  position: absolute;
  z-index: 1;
  color: white;
  margin: -100px 0 0 1400px;
}
.border {
  border-radius: 20px;
}
</style>
