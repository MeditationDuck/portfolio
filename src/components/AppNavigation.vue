<template>
  <v-card
    color="grey lighten-4"
    flat
    height="48px"
    tile
  >
    <v-navigation-drawer app v-model="drawer" dark disable-resize-watcher>
      <v-list>
        <template v-for="(item,index) in items">
          <v-list-tile :key="index">
            <v-list-content>
              {{ item.title }}
            </v-list-content>
          </v-list-tile>
          <v-devider :key="`devider-${index}`"></v-devider>
        </template>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar dense>
      <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer">
      </v-toolbar-side-icon>
      <router-link to="/">
        <v-toolbar-title to="/">{{ pageTitle }}</v-toolbar-title>
      </router-link>
      <v-spacer></v-spacer>
      <v-btn flat class="hidden-sm-and-down" to="/menu">
        Menu
      </v-btn>
    </v-toolbar>
  </v-card>
</template>

<script>
export default {
  name: 'AppNavigation',
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
