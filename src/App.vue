<template>
  <v-app>
    <app-navigation></app-navigation>
    <v-container transition="slide-x-transition">
      <router-view></router-view>
    </v-container>
  </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';

export default {
  name: 'App',
  components: {
    AppNavigation
  }
};
</script>
<style>
</style>
