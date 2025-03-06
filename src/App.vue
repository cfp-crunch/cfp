<script setup>
import PWABadge from './components/PWABadge.vue'
</script>

<template>
  <div>
    <a href="https://vite.dev" target="_blank">
      <img src="/favicon.svg" class="logo" alt="cfp_crunch logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <nav>
    <RouterLink to="/">Go to Home</RouterLink>
    <RouterLink to="/back">Go Back</RouterLink>
  </nav>
  <main>
    <RouterView />
  </main>
  <PWABadge />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
nav, main {
  border: 2px solid #000;
  margin-bottom: 10px;
  padding: 10px;
}

nav > a + a {
  margin-left: 10px;
}

h2 {
  border-bottom: 1px solid #ccc;
  margin: 0 0 20px;
}
</style>
