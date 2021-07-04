<template>
  <div id="app">
    <Animation />
    <Player1 :name="this.p1.name" :team="this.p1.team" :score="this.p1.score" />
    <Player2 :name="this.p2.name" :team="this.p2.team" :score="this.p2.score" />
    <Round :round="this.round" />
  </div>
</template>

<script>
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
      p1: {
        name: "KaiserD",
        team: "WUL3",
        score: 0,
      },
      p2: {
        name: "Luigi",
        team: "CLUST",
        score: 0,
      },
      round: "Winners Quarters",
    };
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
  color: white;
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
  color: rgb(0, 0, 0);
}

.pInfo {
  position: relative;
  top: 12px;
  font-size: 30px;
}

.teams {
  color: rgb(255, 0, 0);
}

</style>
