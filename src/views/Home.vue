<template>
  <span>
    <home-me></home-me>
    <naoki-details></naoki-details>

  </span>
</template>
<script>
import HomeMe from '@/components/HomeMe';
import NaokiDetails from '@/components/NaokiDetails';

export default {
  name: 'home',
  components: {
    HomeMe,
    NaokiDetails
  }
}
</script>