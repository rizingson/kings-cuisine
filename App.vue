<template>
  <v-app>
    <v-navigation-drawer
      app
      v-model="drawer"
      color="#242526"
      dark
      disable-resize-watcher
    >
      <v-list>
        <template v-for="(el, index) in elements">
          <v-list-tile :key="index" :to="el.title">
            <v-list-tile-content>
              {{ el.title }}
            </v-list-tile-content>
          </v-list-tile>

          <v-divider :key="`divider-${index}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>

    <v-toolbar app color="#242526" dark>
      <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"
        >
      </v-toolbar-side-icon>

      <v-spacer class="hidden-md-and-up"></v-spacer>

      <router-link to="/">
        <v-toolbar-title class="link" to="/">{{ appTitle }}</v-toolbar-title>
      </router-link>

      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn flat class="hidden-sm-and-down" to="/About">About</v-btn>
      <v-btn flat class="hidden-sm-and-down" to="/menu" data-cy="menuBtn"
        >Menu</v-btn
      >
      <v-btn flat class="hidden-sm-and-down" to="/location">Location</v-btn>
    </v-toolbar>
    <v-content transition="slide-x-transition">
      <router-view></router-view>
    </v-content>

    <v-footer app dark height="auto">
      <v-card class="flex" color="#242526" flat tile>
        <v-card-title>
          <strong class="subheading"
            >Carryout:
            <a class="link" href="tel:+1209383983">(209) 383-9838</a></strong
          >

          <v-spacer></v-spacer>

          <v-btn
            class="mx-3"
            dark
            icon
            href="https://www.facebook.com/Kings-Asian-Cuisine-Sushi-Bar-and-Lounge-120944707920061/"
          >
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-title>

        <v-card-actions color="#242526" class="justify-center">
          <strong>rizingson</strong> &nbsp; &copy;2019
        </v-card-actions>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      appTitle: "Kings Asian Cuisine",
      drawer: false,

      elements: [{ title: "About" }, { title: "Menu" }, { title: "Location" }],
      icon: "fab fa-facebook"
    };
  }
};
</script>

<style>
.link,
a {
  color: white;
  text-decoration: none;
}
</style>
