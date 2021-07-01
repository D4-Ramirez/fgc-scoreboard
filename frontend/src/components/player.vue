<template>
  <div id="player">
    <span id="score">{{ score }}</span>
    <div id="info">
      <span id="name">{{ name }}</span>
      <span id="team">{{ team }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Player",
  props: {
    name: String,
    team: String,
    score: Number,
  },
};
</script>

<style></style>
