<template>
  <v-container 
  class="grey lighten-1" 
  fluid
  >
    <v-layout>
      <v-flex 
      class="d-flex flex-column align-center justify-center"
      >
        <span 
        class="skills-title d-none d-sm-block " 
        style="font-size: 70px; margin-top: 40px; margin-bottom: 40px;"
          >PROJECTS
        </span>
        <span 
        class="skills-title black--text d-block d-sm-none" 
        style="font-size: 40px; margin-top: 20px; margin-bottom: 20px;"
          >PROJECTS
        </span>
      </v-flex>
    </v-layout>
    <v-layout 
    <!-- style="margin-left: 10%; margin-right: 10%"
    > -->
      <v-flex class="d-flex flex-wrap justify-center">
          <v-card 
          v-for="(project, index) of projects"
          :key="index"
          flat width="60%" class="ma-2">
            <v-card-title class="d-flex align-center">
                <span>{{project.title}}</span>
                <v-spacer></v-spacer>
                  <v-btn
                  icon
                  :href="project.link"
                  target="__blank"
                  >
                    <v-icon x-large color="grey darken-3">mdi-github</v-icon>
                  </v-btn>
                <v-carousel small hide-delimiters color="grey darken-3" class="mt-4">
                  <v-carousel-item contain v-for="(images, index) of project.images"
                  :key="index"
                  :src="require(`~/${images}`)"
                  ></v-carousel-item>
                  </v-carousel>
            </v-card-title> 
            <v-card-subtitle class="mt-4">{{project.content}}</v-card-subtitle>
          </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>



<style>
.skills-title {
  font-family: 'Roboto', sans-serif;
}
.skills-color {
  background: -webkit-linear-gradient(45deg, #a3cafe, #2546d3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  border-bottom: 5px black;
}
</style>

<script lang="ts">
import Vue from 'vue'
import Projects from '@/json/projects.json'

export default Vue.extend({
    data: () => ({
        projects: Projects,
        carousel: 0
    })
})
</script>
