<template>
  <div class="main-video" ref="mainVideo">
    <button class="main-button" @click="hideVideo()">
      Continuer sur le site
    </button>
    <video class="video" autoplay muted loop>
      <source src="../assets/main-video.mp4" type="video/mp4" />
    </video>
  </div>
</template>

<script>
export default {
  methods: {
    hideVideo() {
      this.$refs.mainVideo.classList.add("main-hide");
      document.body.classList.remove("no-scroll");
      scrollTo(0, 0);
    },
  },
};
</script>

<style>
</style>