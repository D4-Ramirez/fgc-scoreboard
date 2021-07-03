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
        name: "D4",
        team: "CLUST",
        score: 0,
      },
      p2: {
        name: "Luigi",
        team: "CLUST",
        score: 0,
      },
      round: "Money Match FT15",
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
</style>
