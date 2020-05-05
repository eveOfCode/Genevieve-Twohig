<template>
  <v-container>
    <h1
      style="text-align: center; font-family: 'Lucida Console', Courier, monospace; letter-spacing: 3px; opacity: 0.91;"
    >
      SKILLS
    </h1>
    <v-layout justify-center align-center row wrap>
      <v-card class="mt-4" shaped width="700px">
        <v-container>
          <v-layout
            justify-center
            align-center
            row
            wrap
            style="padding-left: 100px"
          >
            <v-flex lg6 v-for="(skill, index) in Skills.skills" :key="index">
              <v-list-item>
                <v-list-item-avatar
                  ><img :src="skill.image"
                /></v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title v-text="skill.name"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-flex>
          </v-layout>
        </v-container>
      </v-card>
    </v-layout>
  </v-container>
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
