<template>
  <div id="player1">
    <div id="p1SBox" class="sBoxes">
      <span id="p1Score" class="scores">{{ score }}</span>
    </div>
    <div id="p1IBox" class="iBoxes">
      <div id="p1Info" class="pInfo">
        <span id="p1Team" class="teams">{{ team }}</span>
        <span id="p1Name" class="names">{{ name }}</span>
      </div>
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
#p1SBox {
  left: 574.227px;
}

#p1IBox {
  left: 147.175px;
}
</style>
