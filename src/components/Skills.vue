<template>
  <div style="height:100vh" class="">
    <v-container fluid>
      <v-layout justify-center align-center row wrap>
        <v-card class="mx-2 mt-4" shaped width="900px">
          <v-card-title class="display-2 font-weight-light" text-center
            >Skills</v-card-title
          >
          <v-list>
            <v-list-item v-for="(skill, index) in Skills.skills" :key="index">
              <v-list-item-avatar><img :src="skill.image"/></v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title v-text="skill.name"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-card>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import Skills from "../data/skills.json";
export default {
  data() {
    return {
      Skills
    };
  }
};
</script>
