<template>
  <v-card 
    color="grey lighten-4"
    flat
    height="48px"
    tile
  > 
    <v-toolbar dense> 
      <v-spacer></v-spacer>
      <router-link to="/">
        <v-toolbar-title to="/">{{ pageTitle }}</v-toolbar-title>
      </router-link>
      <v-spacer></v-spacer>
      <!-- <v-btn to="/menu">
        Menu
      </v-btn> -->
    </v-toolbar>
  </v-card>
</template>

<script>
export default {
  name: "AppNavigation",
  data() {
    return {
      pageTitle: 'YoshidaNaoki',
      drawer: false,
      items: [
        { title: "Menu" },
        { title: "About" }
      ]
    }
  }
};
</script>

<style scoped>
a {
  color: black;
  text-decoration: none;
}
.router-link-exact-active {
  color: black;
  text-decoration: none;
}
.v-toolbar__title {
  color: black;
  text-decoration: none;
}
</style>
