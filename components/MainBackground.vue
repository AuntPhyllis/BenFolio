<template>
  <div>
    <!-- <div class="background blue-purple"></div>
    <div class="background green-blue"></div> -->

    <div class="background">
      <img :scr="require('@/assets/Logo/Logo.svg')" class="logo-outline"/>

    </div>
  </div>
</template>

<style>
html,
body {
  height: 100%;
  width: 100%;
}

.background {
  height: 100vh;
  width: 100vw;
  
}

.blue-purple {
  background-color: #000428;
  background-image: -webkit-linear-gradient(left, #587cb3, #000428);
  background-image: linear-gradient(to right, #587cb3, #000428);
  -webkit-animation: fadeInOut 25s ease;
  -moz-animation: fadeInOut 25s ease;
  animation: fadeInOut 25s ease;
  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
  -webkit-animation-iteration-count: infinite;
  -moz-animation-iteration-count: infinite;
  animation-iteration-count: infinite;
}

.green-blue {
  background-color: #bdc3c7;
  background-image: -webkit-linear-gradient(left, #bdc3c7, #2c3e50);
  background-image: linear-gradient(to right, #bdc3c7, #2c3e50);
  -webkit-animation: fadeOutIn 25s ease;
  -moz-animation: fadeOutIn 25s ease;
  animation: fadeOutIn 25s ease;
  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
  -webkit-animation-iteration-count: infinite;
  -moz-animation-iteration-count: infinite;
  animation-iteration-count: infinite;
}

@-webkit-keyframes fadeInOut {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@-moz-keyframes fadeInOut {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@keyframes fadeInOut {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOutIn {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@-moz-keyframes fadeOutIn {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes fadeOutIn {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
.svg-wrapper {
  height: 100vh;
  width: 100vw;

}

#logo-filled {
  fill: #fff;
  opacity: 0;
  -webkit-animation: fadeIn 2s ease;
  -moz-animation: fadeIn 2s ease;
  animation: fadeIn 2s ease;
  -webkit-animation-delay: 2s;
  -moz-animation-delay: 2s;
  animation-delay: 2s;
  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#logo-outline {
  stroke: rgba(255, 255, 255, 0.5);
  stroke-width: 1.25px;
  -webkit-animation: fadeOut 1s ease;
  -moz-animation: fadeOut 1s ease;
  animation: fadeOut 1s ease;
  -webkit-animation-delay: 2.75s;
  -moz-animation-delay: 2.75s;
  animation-delay: 2.75s;
  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}
</style>

<script>
import Vue from "vue";
import Vivus from "vivus";

export default {
  mounted() {
    new Vivus("logo-outline", {
      type: "delayed",
      duration: 200,
      animTimingFunction: Vivus.EASE_OUT,
    });
  },
};
</script>
