<template>
  <div id="player">
    <div id="scWrapper">
      <span id="score">{{ score }}</span>
    </div>
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

<style>
#scWrapper {
  width: 70.5px;
  height: 50px;
  left: 574.227px;
  top: 62px;
  position: absolute;
}

#score {
  position: relative;
  top: 10px;
  font-size: 40px;
  color: black;
}
</style>
