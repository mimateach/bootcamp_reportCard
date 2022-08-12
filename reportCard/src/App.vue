<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue';
</script>

<template>
<Header />

  <RouterView />
</template>

<style scoped>

template {
  width: 100%;
}

</style>
