<script setup>
import StudentData from "../components/StudentData.vue";
import DataTable from "../components/DataTable.vue";
import HomeView from "./HomeView.vue";
</script>

<template>
  <main>

      <div class="dataTable">
        <DataTable />
      </div>
    <div class="button">
      <button>
        <RouterLink to="/">Go back</RouterLink>
      </button>
    </div>
  </main>

  <RouterView />
</template>

<style lang="scss" scoped>

.dataTable {
  height: auto;
  margin-top: 10vh;
}

.button {
  display: flex;
  justify-content: center;
  margin-top: 5vh;
}
button {
  width: 10vw;
  height: 3vh;
}
</style>
