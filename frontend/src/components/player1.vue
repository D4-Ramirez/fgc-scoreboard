<template>
  <div id="player">
    <span id="score">{{ score }}</span>
    <div id="info">
      <span id="team">{{ team }}</span>
      <span id="name">{{ name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Player1",
  props: {
    name: String,
    team: String,
    score: Number,
  },
};
</script>

<style></style>
