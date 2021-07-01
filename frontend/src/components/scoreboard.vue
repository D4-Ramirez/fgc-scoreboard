<template>
  <div id="scoreboard">
    <Player :name="p1.name" :team="p1.team" :score="p1.score" />
    <Player :name="p2.name" :team="p2.team" :score="p2.score" />
    <div id="round">{{ round }}</div>
  </div>
</template>

<script>
import Player from "./player.vue";

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
    Player,
  },
};
</script>

<style></style>
