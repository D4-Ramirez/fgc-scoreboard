<template>
  <div id="animation">
    <lottie-animation
      ref="anim"
      :animationData="require('../assets/animations/data.json')"
      :loop="false"
      :autoPlay="true"
    />
  </div>
</template>

<script>
import LottieAnimation from "lottie-web-vue";

export default {
  name: "Animation",
  components: {
    LottieAnimation,
  },
};
</script>

<style>
#animation {
  z-index: 2;
}
</style>
