<template>
  <v-container>
    <h1>Work</h1>
    <v-layout justify-center text-center wrap row>
      <v-card
        shaped
        class="mx-2"
        v-for="(job, index) in Work.jobs"
        :key="index"
      >
        <v-img :src="job.image" class="white--text align-end" height="500px">
          <v-card-title class="display-1 d-inline">{{
            job.company
          }}</v-card-title>
        </v-img>
        <v-card-text class="subtitle-1">{{ job.description }}</v-card-text>
      </v-card>
    </v-layout>
  </v-container>
</template>

<script>
import Work from "../data/work.json";
export default {
  data() {
    return {
      Work
    };
  }
};
</script>
