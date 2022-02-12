<template>
<!-- Restera toujours affiché -->
<HeaderVue></HeaderVue>
  <router-view />
  <FooterVue></FooterVue>
  <Video></Video>
  <!-- Commence a changer suite au router-view -->
</template>
<script>
import HeaderVue from "./components/Header.vue";
import FooterVue from "./components/Footer.vue";
import Video from "./components/Video.vue";
// @ is an alias to /src       

// Créer un compenant LastArticle
// Créer un compenant PopularArticle
// Créer un compenant Footer
export default {
  name: "App",
  components: {
    HeaderVue,
    FooterVue,
    Video
},
};
</script>
<style>

</style>