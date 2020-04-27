<template>
  <div style="height:100vh" class="">
    <v-container fill-height>
      <v-layout justify-center align-center text-center row>
        <v-card><v-card-text>asdkfjkhjsdfj askdjkfasjdfh</v-card-text></v-card>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import Parser from "rss-parser";
export default {
  data: () => ({}),
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
    // axios.get("/api/", result => {
    //   // eslint-disable-next-line no-console
    //   console.log(result);
    // });
  }
};
</script>
