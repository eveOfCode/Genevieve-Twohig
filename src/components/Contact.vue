<template>
  <div style="height:90vh" class="mt-5">
    <v-container fill-height height="100vh">
      <v-layout align-center justify-center text-center wrap row>
        <v-flex lg6 sm12>
          <v-card class="rounded_card ml-4">
            <h1 class="section_headers pa-2">{{ Contact.section_title }}</h1>
            <v-card-text>{{ Contact.text }} </v-card-text>

            <h2 style="color:rgba(255, 99, 71, 0.5); margin-bottom: 15px;">
              <span style="color: grey; font-size: 14px;">email:</span>
              {{ Contact.email }}
            </h2>

            <v-btn
              icon
              target="blank"
              :href="Contact.linkedin_link"
              class="mb-4"
            >
              <v-icon color="blue" large>fab fa-linkedin</v-icon>
            </v-btn>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import Contact from "../data/contact.json";
export default {
  data() {
    return {
      Contact
    };
  }
};
</script>
