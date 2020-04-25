<template>
  <div style="height:100vh" class="">
    <v-container>
      <h1>Skills</h1>
      <v-layout justify-center wrap row>
        <!-- <v-flex lg4> -->
        <v-card class="mx-2" shaped width="800px">
          <v-list>
            <v-list-item v-for="(skill, index) in Skills.skills" :key="index">
              <v-list-item-icon>
                <v-avatar><img :src="skill.image"/></v-avatar>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title v-text="skill.name"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-card>
        <!-- </v-flex> -->
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
