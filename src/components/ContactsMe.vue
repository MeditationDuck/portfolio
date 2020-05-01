<template>
  <v-footer dark padless height='200px'>
      <v-card
        color="rgb(255, 0, 0, 0)"
        flat
        tile
        width="100%"
        class="text-center"
      >
        <v-btn
          v-for="(item, i) in items"
          :key="i"
          :href="item.link"
          class="mx-3 white--text"
          icon
        >
          <v-icon size="30px">{{ item.icon }}</v-icon>
        </v-btn>
       </v-card>
      <v-card-text class="white--text pt-0">
        Koreha 'NaokiYoshida' no potoforio dayo, byuujyeies ha sugoku kantanni kireini dekirune.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text text-center">
          {{ new Date().getFullYear() }} — <strong>NaokiYoshida.</strong>
      </v-card-text>
  </v-footer>
</template>

<script>
export default {
  name: "ContactsMe",
   data: () => ({
      items: [
        {
          link: 'https://github.com/MeditationDuck',
          icon: 'mdi-github',
        },
        {
          link: 'https://www.instagram.com/meditationduck/',
          icon: 'mdi-instagram',
        },
        {
          link: 'https://twitter.com/Meditation_Duck',
          icon: 'mdi-twitter',
        },
        {
          link: 'https://www.facebook.com/naoki.yoshida.796774',
          icon: 'mdi-facebook',
        },
        {
          link: 'mailto:dw9t5j9@gmail.com?body=%E6%84%8F%E8%A6%8B%EF%BC%8C%E8%B3%AA%E5%95%8F%EF%BC%8C%E3%81%8A%E4%BB%95%E4%BA%8B%EF%BC%8C%E3%81%AA%E3%81%A9%E3%81%82%E3%82%8A%E3%81%BE%E3%81%97%E3%81%9F%E3%82%89%E3%81%A9%E3%81%86%E3%81%9E%EF%BC%8E%0D%0A%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%EF%BC%9D%0D%0A%0D%0A%E5%90%8D%E5%89%8D%EF%BC%9A%0D%0A%E3%81%8A%E5%95%8F%E3%81%84%E5%90%88%E3%82%8F%E3%81%9B%E5%86%85%E5%AE%B9%EF%BC%9A%0D%0A',
          icon: 'mdi-email',
        },
      ],
    }),
};
</script>