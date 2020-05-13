<template>
  <div style="height:60vh" class="mt-5">
    <v-container>
      <h1 class="section_headers mb-4">{{ About.section_title }}</h1>
      <v-layout justify-center row wrap>
        <v-flex lg5 md8 sm8 xs12 class="px-4">
          <p style="color: grey">{{ About.text }}</p>
        </v-flex>
        <v-flex lg4 md4 sm8 xs12 class="px-4" align-self-center="">
          <v-card class="pa-4 rounded_card" max-width="400" max-height="350">
            <v-flex>
              <v-card max-width="373" max-height="280" class="rounded_card"
                ><v-img :src="About.image" height="280" width="373"
              /></v-card>
            </v-flex>
            <v-card-subtitle class="text-center">{{
              About.image_subtitle
            }}</v-card-subtitle>
          </v-card>
        </v-flex>
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
