<template>
  <nav class="nav">
    <svg class="nav-icon" viewBox="0 0 100 80">
      <rect width="100" height="20" rx="8"></rect>
      <rect y="30" width="100" height="20" rx="8"></rect>
      <rect y="60" width="100" height="20" rx="8"></rect>
    </svg>
    <ul class="nav-list">
      <li class="nav-item">
        <router-link class="nav-link" to="/">Accueil</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/">Blog</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/">À propos</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/contact">Contact</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
};
</script>

<style>
</style>