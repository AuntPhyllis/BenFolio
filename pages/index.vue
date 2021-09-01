<template>
  <div>
      <Header float logo />
      <v-img
      width="100%"
      height="100vh"
      :src="require('@/assets/Background.png')"
      >  
        <v-layout 
        column 
        fill-height 
        justify-center 
        align-center
        style="background-color: rgba(0,0,0,0.4)"
        >
        <div class="px-3">
          <span class="
          text-h3
          text-sm-h2
          text-md-h2
          text-lg-h1
          font-weight-thin
          white--text
          "><span class="font">BEN TALBOT</span></span>
            <span class="
            d-block
            text-center
            text-h6 
            text-sm-h6 
            text-md-h5 
            text-lg-h4 
            white--text
            ">Full Stack | Developer | Designer</span>
          </div>
        </v-layout>
      </v-img>
      <About />
      <Skills />
      <Projects />
    
  </div> 
</template>



