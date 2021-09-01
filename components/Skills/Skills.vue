<template>
  <v-container 
  class="grey lighten-2" 
  fluid
  >
    <v-layout>
      <v-flex 
      class="d-flex flex-column align-center justify-center"
      >
        <span 
        class="skills-title d-none d-sm-block " 
        style="font-size: 70px; margin-top: 40px; margin-bottom: 40px;"
          >TECHNOLOGIES
        </span>
        <span 
        class="skills-title black--text d-block d-sm-none" 
        style="font-size: 40px; margin-top: 20px; margin-bottom: 20px;"
          >TECHNOLOGIES
        </span>
      </v-flex>
    </v-layout>
    <v-layout 
    style="margin-left: 12vw; margin-right: 12vw"
    >
      <v-flex class="d-flex flex-wrap justify-center">
          <v-card 
          v-for="(item, index) of skills"
          :key="index"
          flat max-width="400px" class="ma-2">
            <v-card-title class="d-flex align-center">
                <span>{{item.title}}</span>
                <v-spacer></v-spacer>
                <v-icon x-large color="grey darken-3">{{item.icon}}</v-icon>
            </v-card-title> 
            <v-card-subtitle style="margin-top: 0.5vw;">{{item.content}}</v-card-subtitle>
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
import skills from '@/json/skills.json'

export default Vue.extend({
    data: () => ({
        skills
    })
})
</script>
