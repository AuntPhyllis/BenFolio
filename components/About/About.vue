<template>
<v-container style="height: 100vh" class="grey lighten-3" fluid>
  <v-layout fill-height class="d-sm-none">
        <v-flex class="d-flex flex-column align-center justify-center">
          <v-avatar
          class="profile elevation-12 d-sm-none"
          size="200"
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >
            </v-img>
        </v-avatar>
          <span 
          class="about-title black--text"
          style="font-size: 20px; margin-top: 40px;"
          >LETS MAKE SOMETHING
          </span>
          <span 
          class="about-title about-color"
          style="font-size: 51px; margin-top: -20px;"
          >AMAZING
          </span>
          <span
          class="black--text text-center"
          >Hi! I'm Ben, a developer based in the greater Calgary metropolitan area.
          </span>
          <br>
          <span
          class="black--text text-center"
          >I am a systematic and personable software development graduate. I value the peace of mind of my 
           coworkers and clients by utilizing practical and thoughtful solutions to analytical problems.
           <br><br>
           I am seeking to apply my expertise to build a lucrative and lasting career as a full stack 
           software developer
          </span>
       </v-flex>
    </v-layout>
    <v-layout fill-height style="margin-left: 12vw; margin-right: 12vw;">
        <v-flex 
        class="d-flex flex-column align-center justify-center"
        >
          <span 
          class="about-title black--text d-none d-md-block"
          style="font-size: 50px;"
          contain
          >LETS MAKE SOMETHING</span>
          <span 
          class="about-title black--text d-none d-sm-block d-md-none"
          style="font-size: 20px;"
          contain
          >LETS MAKE SOMETHING</span>

          <span 
          class="about-title about-color d-none d-md-block"
          style="font-size: 130px; margin-top: -50px;"
          contain
          >AMAZING</span>
          <span 
          class="about-title about-color d-none d-sm-block d-md-none"
          style="font-size: 50px; margin-top: -20px;"
          contain
          >AMAZING</span>

          <span
          class="black--text text-center d-none d-md-block"
          style="font-size: 21px;"
          >Hi! I'm Ben, a developer based in the greater Calgary metropolitan area.
          I am a systematic and personable software development graduate. I value the peace of mind of my 
           coworkers and clients by utilizing practical and thoughtful solutions to analytical problems.
           <br><br>
           I am seeking to apply my expertise to build a lucrative and lasting career as a full stack 
           software developer.
          </span>
          <span
          class="black--text text-center d-none d-sm-block d-md-none"
          style="font-size: 11px;"
          >Hi! I'm Ben, a developer based in the greater Calgary metropolitan area.
          I am a systematic and personable software development graduate. I value the peace of mind of my 
           coworkers and clients by utilizing practical and thoughtful solutions to analytical problems.
           <br><br>
           I am seeking to apply my expertise to build a lucrative and lasting career as a full stack 
           software developer.
          </span> 

          <br>
          <span class="d-flex justify-space-between">
            <v-btn >Contact Me</v-btn>
            <v-btn>View Resume</v-btn>
          </span>
        </v-flex>
        <v-flex 
        class="d-flex align-center justify-center"
        style="margin-left: 12vw;"
        >
          <v-avatar
          class="profile elevation-12 d-none d-md-block"
          size="560"
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >
            </v-img>
        </v-avatar>
        <v-avatar
          class="profile elevation-12 d-none d-sm-block d-md-none"
          size="220"
          >
            <v-img
            :src="require('@/assets/AvatarFull.jpg')"
            >
            </v-img>
        </v-avatar>
        </v-flex>
    </v-layout>
</v-container>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@900&display=swap');

.about-title {
  font-family: 'Heebo', sans-serif;
}
.about-color {
  background: -webkit-linear-gradient(45deg, #A3CAFE, #2546D3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  border-bottom: 5px black;
}
</style>