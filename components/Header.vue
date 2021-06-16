<template>
  <v-app-bar color="transparent" flat :absolute="float">
    <v-toolbar-title class="font">
      <v-btn text plain to="/">Ben Talbot</v-btn>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn text to="/projects">Projects</v-btn>
      <v-btn text href="/resume.pdf" target="__blank">Resume</v-btn>
    </v-toolbar-items>
  </v-app-bar>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  props: {
    logo: Boolean,
    float: Boolean,
  },
});
</script>