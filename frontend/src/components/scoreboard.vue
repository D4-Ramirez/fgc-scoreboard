<template>
  <div id="scoreboard">
    <Animation />
    <Player1 :name="p1.name" :team="p1.team" :score="p1.score" />
    <Player2 :name="p2.name" :team="p2.team" :score="p2.score" />
    <div id="round">{{ round }}</div>
  </div>
</template>

<script>
import Player1 from "./player1.vue";
import Player2 from "./player2.vue";
import Animation from "./animation.vue";

export default {
  name: "Scoreboard",
  props: {
    p1: {
      name: String,
      team: String,
      score: Number,
    },
    p2: {
      name: String,
      team: String,
      score: Number,
    },
    round: String,
  },
  components: {
    Player1,
    Player2,
    Animation,
  },
};
</script>

<style>
/* #scoreboard {
  text-align: center;
  color: white;
  font-size: 30px;
}
#round {
  height: 48.6px;
  width: 272.7px;
  top: 5px;
  left: 823.655px;
  position: absolute;
} */
</style>
