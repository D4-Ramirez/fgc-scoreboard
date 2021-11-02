<template>
  <div id="app">
    <Animation />
    <Player1 :name="data.p1Name" :team="data.p1Team" :score="data.p1Score" />
    <Player2 :name="data.p2Name" :team="data.p2Team" :score="data.p2Score" />
    <Round :round="data.round" />
  </div>
</template>

<script>
import json from "./assets/streamcontrol.json";
import gsap from "gsap";
import Player1 from "./components/player1.vue";
import Player2 from "./components/player2.vue";
import Round from "./components/round.vue";
import Animation from "./components/animation.vue";

export default {
  name: "App",
  components: {
    Player1,
    Player2,
    Round,
    Animation,
  },
  data() {
    return {
      data: json,
    };
  },
  mounted() {
    this.startAnimation();
  },
  methods: {
    startAnimation() {
      gsap.to(".scores", {
        css: { opacity: 1 },
        ease: "Quad.easeOut",
        delay: 1,
      });
      gsap.to("#round", {
        css: { opacity: 1 },
        ease: "Quad.easeOut",
        delay: 1,
      });
      gsap.to(".pInfo", {
        css: { opacity: 1 },
        ease: "Quad.easeOut",
        delay: 1,
      });
    },
  },
};
</script>

<style>
body {
  width: 1920px;
  height: 1080px;
  text-align: center;
  overflow: hidden;
  margin: 0px;
  padding: 0px;
  color: rgb(255, 255, 255);
  font-family: "Josefin Sans", sans-serif;
}

.sBoxes {
  position: absolute;
  width: 70.5px;
  height: 50px;
  top: 62px;
}

.iBoxes {
  position: absolute;
  width: 427.1px;
  height: 50px;
  top: 62px;
}

.scores {
  position: relative;
  top: 9px;
  font-size: 40px;
  opacity: 0;
  color: rgb(0, 0, 0);
}

.pInfo {
  position: relative;
  top: 12px;
  font-size: 30px;
  opacity: 0;
}

.teams {
  color: rgb(53, 91, 128);
}
</style>
