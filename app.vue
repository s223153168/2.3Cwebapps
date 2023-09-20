<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="app">
    <header>
      <div class="wrapper">
        <h1>The Weeknd World Tour</h1>
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/tour-dates">Tour Dates</RouterLink>
        </nav>
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
/* Keep the existing styles and add new styles as needed for the website's look and feel */
.app {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
}

header {
  background-color: #000;
  color: #fff;
  padding: 20px 0;
  text-align: center;
}

.wrapper {
  max-width: 1200px;
  margin: 0 auto;
}

h1 {
  font-size: 2rem;
  margin: 0;
}

nav {
  margin-top: 10px;
}

nav a {
  margin-right: 20px;
  text-decoration: none;
  color: #fff;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}
</style>
