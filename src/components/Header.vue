<template>
  <header class="header">
    <h1 class="main-title">Xin chào Vietnam</h1>
    <NavVue></NavVue>
  </header>
</template>

<script>
//j'ai importé un objet NavVue depuis .Nav.vue pui j'ai déclaré NavVue dans mes components
import NavVue from "./Nav.vue";
export default {
  name: "Header",
  components: {
    NavVue,
  },
};
</script>

<style>
</style>