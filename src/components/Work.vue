<template>
  <!-- style="height:150vh" -->
  <div style="height:100vh">
    <v-container>
      <h1 class="section_headers">
        WORK
      </h1>
      <v-layout justify-center text-center row wrap>
        <v-flex
          lg6
          md8
          sm8
          xs12
          class="mt-4 px-4"
          v-for="(job, index) in Work.jobs"
          :key="index"
        >
          <v-card class="rounded_card">
            <v-img
              :src="job.image"
              class="white--text align-end"
              height="500px"
            >
              <!-- d-inline -->
              <v-card-title class="display-1 d-inline">{{
                job.company
              }}</v-card-title>
            </v-img>
            <v-card-text class="subtitle-1" style="text-align: left;">{{
              job.description
            }}</v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
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
