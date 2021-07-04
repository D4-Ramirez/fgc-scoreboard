<template>
  <div id="rdWrapper">
    <div id="round">{{ round }}</div>
  </div>
</template>

<script>
export default {
  name: "Round",
  props: {
    round: String,
  },
};
</script>

<style>
#rdWrapper {
  position: absolute;
  width: 273px;
  height: 48.6px;
  left: 822.7px;
  top: 5px;
}

#round {
  position: relative;
  top: 8px;
  font-size: 27px;
  opacity: 0;
}
</style>
