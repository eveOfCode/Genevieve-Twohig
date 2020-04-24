<template>
  <v-container>
    <h1>Skills</h1>
    <v-layout justify-center text-center wrap row>
      <v-flex lg4>
        <v-card class="mx-2">
          <span>
            <!-- <v-avatar>
              <v-img src="https://thispersondoesnotexist.com/image"></v-img>
            </v-avatar> -->
            <v-avatar size="60" tile class="mt-5">
              <v-img src="https://vuejs.org/images/logo.png" />
            </v-avatar>
          </span>
          <v-card-title>Programming Languages</v-card-title>
          <v-card-text
            >asdkjfkajsdf; asdjkfl;ak asdfkj asdjf;ak akdfl</v-card-text
          >
        </v-card>
      </v-flex>
      <v-flex lg4>
        <v-card class="mx-2">
          <v-card-title>Web Development</v-card-title>
          <v-card-text
            >asdkjfkajsdf; asdjkfl;ak asdfkj asdjf;ak akdfl</v-card-text
          >
        </v-card>
      </v-flex>
      <v-flex lg4>
        <v-card class="mx-2">
          <v-card-title>Data Analytics</v-card-title>
          <v-card-text
            >asdkjfkajsdf; asdjkfl;ak asdfkj asdjf;ak akdfl</v-card-text
          >
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({})
};
</script>
