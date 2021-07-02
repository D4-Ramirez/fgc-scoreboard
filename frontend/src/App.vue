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
        team: "TH",
        score: 0,
      },
      p2: {
        name: "Luigi",
        team: "VG",
        score: 0,
      },
      round: "Grand Finals",
    };
  },
};
</script>

<style></style>
