<script setup>
import StudentData from "../components/StudentData.vue";
import DataTable from "../components/DataTable.vue";
import HomeView from "./HomeView.vue";
</script>

<template>
  <main>
    <div class="studentInfo">
      <div class="studentData">
        <StudentData />
      </div>
      <div class="dataTable">
        <DataTable />
      </div>
    </div>
    <div class="button">
      <button>
        <RouterLink to="./views/HomeView.vue">Go back</RouterLink>
      </button>
    </div>
  </main>

  <RouterView />
</template>

<style lang="scss" scoped>
.studentInfo {
  display: flex;
  justify-content: space-between;
}
.studentData,
.dataTable {
  height: auto;
  margin-top: 10vh;
}
.studentData {
  width: 20vw;
  background-color: #1e2d2d;
  color: #d7fcfc;
  padding: 2vw;
}
.dataTable {
  width: 60vw;
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
