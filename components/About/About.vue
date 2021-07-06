<template>
<v-container style="height: 100vh" class="grey lighten-3" fluid>
    <v-layout fill-height>
        <v-flex class="d-flex flex-column align-center justify-center">
          <span>LETS MAKE SOMETHING</span>
          <span>AMAZING</span>
          <span>blah blah blah blah blah blah blah blah blah blah</span>
       </v-flex>
        <v-flex class="d-flex align-center justify-center">
            <v-avatar
          class="profile elevation-12"
          size="564"
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >
            </v-img>
        </v-avatar>
        </v-flex>
    </v-layout>
</v-container>
    <!-- <v-container
      width="100%"
      height="100vh"
      class="grey lighten-3">
      <v-layout>
      <div class="d-flex">
        <div class="d-flex flex-column align-center justify-center">
          <span>LETS MAKE SOMETHING</span>
          <span>AMAZING</span>
          <span>blah blah blah blah blah blah blah blah blah blah</span>
        </div>
      <div class="d-flex align-center justify-center">
        <v-avatar
          class="profile elevation-12 mb-12"
          size="564"
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >
            </v-img>
        </v-avatar>
      </div>
      </div>
      </v-layout>
    </v-container> -->

        <!-- <v-container fill-height fluid>
          <v-row>
            <v-col md="1"></v-col>
            <v-col
              md="5"
              class="px-16"
              cols="12"
              align-self="center"
            >
            <div class="d-block">
            <h1 class="text-center black--text about-title">LETS CREATE SOMETHING</h1>
            <h1 class="text-center black--text about-title about-color">AMAZING</h1>
            <h3 class="text-center black--text">BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH BLAH</h3>
            </div>
          
        </v-col>
        <v-col
              md="6"
              class="px-16"
              cols="12"
            >
          <v-avatar
          class="profile elevation-12 mb-12"
          size="564"
          
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >

            </v-img>
          </v-avatar>
        </v-col>
          </v-row>
        </v-container>             -->
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@900&display=swap');

.about-title {
  font-family: 'Heebo', sans-serif;
  font-size: 6vh;
}
.about-color {
  font-size: 16.5vh;
  background: -webkit-linear-gradient(45deg, #A3CAFE, #2546D3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-top: -7vh;
  border-bottom: 5px black;
}
</style>