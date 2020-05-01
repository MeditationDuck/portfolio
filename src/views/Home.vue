<template>
  <span>
    <home-me></home-me>
    <naoki-details></naoki-details>
    <time-line></time-line>
  </span>
</template>
<script>
import HomeMe from '@/components/HomeMe';
import NaokiDetails from '@/components/NaokiDetails';
import TimeLine from '@/components/TimeLine';

export default {
  name: 'home',
  components: {
    HomeMe,
    NaokiDetails,
    TimeLine,
  }
}
</script>