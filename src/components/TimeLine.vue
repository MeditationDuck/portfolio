<template>
  <v-timeline :dense="$vuetify.breakpoint.smAndDown">
    <v-timeline-item
      fill-dot
      v-for="(item, index) in items" :key="index"
      :color="item.color"
    >
      <v-card>
        <v-card-title :class="item.color">
          <v-icon
            dark
            size="42"
            class="mr-4"
          >
            {{ item.icon }}
          </v-icon>
          <h2 class="display-1 white--text font-weight-light">{{item.title}}</h2>
        </v-card-title>
        <v-container>
          <v-row>
            <v-col cols="12" md="10">
              {{item.content}}
            </v-col>
            <v-col
              class="hidden-sm-and-down text-right"
              md="2"
            >
              <!-- <v-icon size="64">mdi-calendar-text</v-icon> -->
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
  name: "TimeLine",
  data() {
    return {
      items:[
        {
          color: "purple",
          icon: "mdi-alarm",
          title: "誕生",
          content:"2002年4月，人間となった．",

        },
        { 
          color: "pink lighten-2",
          icon: "mdi-monitor-multiple",
          title: "テクノロジーに興味を持つ",
          content:"ジャンクPCを触ったことをきっかけに，僕の歴史がスタートした．",

        },
        { 
          color: "red lighten-1",
          icon: "mdi-elevation-rise",
          title: "スパルタキャンプに参加",
          content:"スパルタキャンプUnity編に参加した．オフライン参加系の勉強会は初めてでリアルな仲間が多くできた．",

        },
        {
          color: "green lighten-1",
          icon: "mdi-earth",
          title: "SecHack365に参加",
          content:"SecHack365に参加し，レベルの高い広い世界に圧倒した．",
        },
        {
          color: "green lighten-2",
          icon: " mdi-heart",
          title: "非公式岩手県版コロナウイルス対策サイトの製作",
          content:"最初はわからないことだらけだったが，とにかくやってみよう．だれかの役に立ってほしい．そういう願いから制作を始めた．",
        },
        {
          color: "blue",
          icon: "mdi-source-fork",
          title: "現在",
          content:"自分自身の可能性を広げかつ自分にしかできないことを見つけるために，試行錯誤と挑戦を繰り返している．",
        },
      ]
    }
  }
};
</script>
<style lang="stylus" scoped>

</style>