<template>
  <div id="player1">
    <div id="p1SBox">
      <span id="p1Score">{{ score }}</span>
    </div>
    <div id="p1IBox">
      <div id="p1Info">
        <span id="p1Team">{{ team }}</span>
        <span id="p1Name">{{ name }}</span>
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
  position: absolute;
  width: 70.5px;
  height: 50px;
  left: 574.227px;
  top: 62px;
}

#p1Score {
  position: relative;
  top: 10px;
  font-size: 40px;
  color: black;
}

#p1IBox {
  position: absolute;
  width: 427.1px;
  height: 50px;
  left: 147.175px;
  top: 62px;
}

#p1Info {
  position: relative;
  top: 12px;
  font-size: 30px;
}

#p1Name {
  color: white;
}

#p1Team {
  color: lightseagreen;
}
</style>
