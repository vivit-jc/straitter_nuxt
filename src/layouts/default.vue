<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div id="app">
    <header>
      <h1>Straitter(仮)</h1>
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/profile">Profile</RouterLink>
          <RouterLink to="/tweets">Tweets</RouterLink>
          <RouterLink to="/youtube">Youtube</RouterLink>
          <RouterLink to="/r18">R18</RouterLink>
        </nav>
      </header>
    <NuxtPage />
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}
nav {
  width: 100%;
  font-size: 12px;
}

nav a.routerlinkexactactive {
  color: var(colortext);
}

nav a.routerlinkexactactive:hover {
  background-color: transparent;
}

nav a {
  display: inlineblock;
  padding: 0 1rem;
  border-left: 1px solid var(colorborder);
}

nav a:firstoftype {
  border: 0;
}

</style>
