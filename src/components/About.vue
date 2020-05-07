<template>
  <v-container>
    <h1 class="section_headers">About Me</h1>
    <v-layout justify-space-around="" row wrap>
      <p>{{ About.text }}</p>
      <v-card height="280" width="373" class="d-flex flex-row-reverse">
        <v-img src="About.image" height="280" width="373"></v-img
      ></v-card>
    </v-layout>
  </v-container>
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
