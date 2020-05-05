<template>
  <v-container fill-height>
    <v-layout justify-center text-center wrap row>
      <v-card class="mx-2 rounded_card" width="900px">
        <h1 class="section_headers">Let's Chat! 👋</h1>
        <v-card-text
          >Have any interesting projects in mind? Want to keep up with
          me?</v-card-text
        >
        <v-card-text>Contact me or follow me on LinkedIn!</v-card-text>

        <h2 style="color:rgba(255, 99, 71, 0.5); margin-bottom: 15px;">
          <span style="color: grey; font-size: 14px;">email:</span>
          gen.twohig@gmail.com
        </h2>

        <v-btn
          icon
          target="blank"
          href="https://www.linkedin.com/in/genevieve-twohig-11623615a/"
          class="mb-4"
        >
          <v-icon color="blue" large>fab fa-linkedin</v-icon>
        </v-btn>
      </v-card>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({})
};
</script>
