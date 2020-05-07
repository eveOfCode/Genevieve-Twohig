<template>
  <div style="height:90vh" class="mt-5">
    <v-container>
      <h1 class="section_headers">{{ About.section_title }}</h1>
      <v-layout justify-space-around="" row wrap>
        <p style="color: grey">{{ About.text }}</p>
        <v-card class="pa-4 rounded_card">
          <v-card width="373" height="280" class="rounded_card"
            ><v-img :src="About.image" height="280" width="373"
          /></v-card>
          <v-card-subtitle class="text-center">{{
            About.image_subtitle
          }}</v-card-subtitle>
        </v-card>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import About from "../data/about.json";
export default {
  data() {
    return {
      About
    };
  }
};
</script>
