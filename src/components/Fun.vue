<template>
  <!-- style="height:100vh" -->
  <div class="">
    <v-container>
      <h1 class="section_headers">Blog</h1>
      <v-layout justify-center align-center row>
        <v-card
          width="350px"
          class="mx-5 my-5 rounded_card"
          v-for="(article, index) in Fun.articles"
          :key="index"
        >
          <v-card class="mt-4 mx-5 rounded_card"
            ><v-img height="200px" src="article1_image.png"></v-img
          ></v-card>
          <a
            style="text-decoration: none; color: black; "
            :href="article.link"
            target="blank"
          >
            <h3 style="padding-left:15px; padding-top: 8px">
              {{ article.title }}
            </h3>
          </a>
          <span style="padding-left:15px; font-size:15px; color:grey;">
            {{ article.subtitle }} <br />
          </span>
          <span
            style="padding-left:15px; padding-right: 3px; font-size:15px; color:grey;"
          >
            {{ article.date_published }}
          </span>
          <div class="circle"></div>
          <span style="padding-left:3px; font-size:15px; color:grey;">
            {{ article.read_length }}
          </span>
          <v-card-text>{{ article.description }}</v-card-text>
          <v-btn class="mx-4 my-5" target="blank" :href="article.link">Read more</v-btn>
        </v-card>
      </v-layout>
    </v-container>
    <v-container>
      <h1 class="section_headers">Cool Events I've Gone To</h1>
      <v-layout justify-center align-center row>
        <v-flex
          lg6
          class="pa-2 "
          v-for="(event, index) in Fun.events"
          :key="index"
        >
          <v-img :src="event.image" contain width="500px" />
          <v-card-title>{{ event.name }}</v-card-title>
          <v-card-text style="color: grey">{{ event.text }}</v-card-text>
          <v-btn target="blank" :href="event.link" class="mx-4"
            >Read more</v-btn
          >
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import Fun from "../data/fun.json";
import Parser from "rss-parser";
export default {
  data() {
    return {
      Fun
    };
  },
  mounted() {
    let parser = new Parser();

    (async () => {
      let feed = await parser.parseURL("/api");
      // eslint-disable-next-line no-console
      console.log(feed.title);

      feed.items.forEach(item => {
        // eslint-disable-next-line no-console
        console.log(item);
      });
    })();
  }
};
</script>
<style>
.circle {
  height: 5px;
  width: 5px;
  background-color: #555;
  border-radius: 50%;
  display: inline-block;
  vertical-align: middle;
}
</style>
