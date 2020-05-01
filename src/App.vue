<template>
  <v-app>
    <app-navigation></app-navigation>
    <v-container transition="slide-x-transition">
      <router-view></router-view>
    </v-container>
    <contacts-me></contacts-me>
  </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
import ContactsMe from '@/components/ContactsMe';

export default {
  name: 'App',
  components: {
    AppNavigation,
    ContactsMe,
  }
};
</script>
<style>
</style>
