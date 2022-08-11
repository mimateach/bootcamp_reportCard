<script setup>
import Header from "../components/Header.vue";
</script>

<template>
  <main>
    <Header />
    <h3>
      You’ve successfully created a project with
    </h3>
        <h3>
      You’ve successfully created a project with
      <a target="_blank" href="https://vitejs.dev/">Vite</a> +
      <a target="_blank" href="https://vuejs.org/">Vue 3</a>.
    </h3>

  </main>
  <RouterView />
</template>

<style lang="scss" scoped>
h3 {
    color: blue;
}
</style>