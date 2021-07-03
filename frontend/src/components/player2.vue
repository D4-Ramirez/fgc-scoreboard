<template>
  <div id="player1">
    <div id="p2SBox">
      <span id="p2Score">{{ score }}</span>
    </div>
    <div id="p2IBox">
      <div id="p2Info">
        <span id="p2Team">{{ team }}</span>
        <span id="p2Name">{{ name }}</span>
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
#p2SBox {
  position: absolute;
  width: 70.5px;
  height: 50px;
  left: 1275.5px;
  top: 62px;
}

#p2Score {
  position: relative;
  top: 10px;
  font-size: 40px;
  color: black;
}

#p2IBox {
  position: absolute;
  width: 427.1px;
  height: 50px;
  left: 1346.05px;
  top: 62px;
}

#p2Info {
  position: relative;
  top: 12px;
  font-size: 30px;
}

#p2Name {
  color: white;
}

#p2Team {
  color: lightseagreen;
}
</style>
