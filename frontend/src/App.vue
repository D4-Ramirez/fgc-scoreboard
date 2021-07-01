<template>
  <div id="app">
    <scoreboard :round="round" :p1="p1" :p2="p2" />
  </div>
</template>

<script>
import Scoreboard from "./components/scoreboard.vue";

export default {
  name: "App",
  components: {
    Scoreboard,
  },
  data() {
    return {
      p1: {
        name: "D4",
        score: 0,
        team: "CLUST",
      },
      p2: {
        name: "Luigi",
        score: 0,
        team: "CLUST",
      },
      round: "Grand Finals",
    };
  },
};
</script>

<style></style>
