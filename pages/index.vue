<template>
  <div class="container">
    <img src="~/assets/images/IMG_8229_square.jpg"/>
    <h2>
      <vue-typer
        text=""
        :erase-on-complete='false'
        :text="['Hello I\'m Jaume 👋','I\'m a full stack web developer based in London 🇬🇧', 'Thanks for passing by, I hope you have a fantastic day 😊']"
      ></vue-typer>
    </h2>

  </div>

</template>

<script>

import backgroundUrl from '~/assets/back-rect-4.jpg';
import Terminal from "../components/Terminal";

export default {

  components: {
    Terminal
  },
  data() {
    return {backgroundUrl};
  }

}
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding-top: 15rem;

}


.row {
  text-align: center;
}

img {
  border-radius: 50%;
  width: 20%;
}

h2 {
  padding-top: 2rem;
}

.wave {
  animation-name: wave-animation; /* Refers to the name of your @keyframes element below */
  animation-duration: 2.5s; /* Change to speed up or slow down */
  animation-iteration-count: infinite; /* Never stop waving :) */
  transform-origin: 70% 70%; /* Pivot around the bottom-left palm */
  display: inline-block;
}

@keyframes wave-animation {
  0% {
    transform: rotate(0.0deg)
  }
  10% {
    transform: rotate(14.0deg)
  }
  /* The following five values can be played with to make the waving more or less extreme */
  20% {
    transform: rotate(-8.0deg)
  }
  30% {
    transform: rotate(14.0deg)
  }
  40% {
    transform: rotate(-4.0deg)
  }
  50% {
    transform: rotate(10.0deg)
  }
  60% {
    transform: rotate(0.0deg)
  }
  /* Reset for the last half to pause */
  100% {
    transform: rotate(0.0deg)
  }
}

</style>
