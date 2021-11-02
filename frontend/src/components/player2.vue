<template>
  <div id="player2">
    <div id="p2SBox" class="sBoxes">
      <span id="p2Score" class="scores">{{ score }}</span>
    </div>
    <div id="p2IBox" class="iBoxes">
      <div id="p2Info" class="pInfo">
        <span id="p2Team" class="teams">{{ team }} </span>
        <span id="p2Name" class="names">{{ name }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Player2",
  props: {
    name: String,
    team: String,
    score: String,
  },
};
</script>

<style>
#p2SBox {
  left: 1275.5px;
}

#p2IBox {
  left: 1346.05px;
}
</style>
