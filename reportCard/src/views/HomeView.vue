<script setup>
import MarksView from "@/views/MarksView.vue";
</script>

<template>
  <main>
    <button>
      <RouterLink to="./views/MarksView.vue">Go to mark's reports</RouterLink>
    </button>
    
  </main>
</template>

<style scoped>
  main {
    display: flex;
    justify-content: center;
    margin: 10vh 0 10vh 0;
  }
  button {
    height: 5vh;
    background-color: transparent;
    border-radius: 10px;
    border: solid gray 0.1vh;
    box-shadow: 3px 3px 2px #406868;
  }
</style>