<!-- eslint-disable vue/no-export-in-script-setup -->
<script>
export default {
  data() {
    return {
      marks: [
        {
          id: 1,
          name: "Paige",
          History: 4,
          Spanish: 6,
          English: 9,
          Science: 2,
        },
        {
          id: 2,
          name: "Alan",
          History: 2,
          Spanish: 8,
          English: 5,
          Science: 9,
        },
        {
          id: 3,
          name: "Oliver",
          History: 1,
          Spanish: 6,
          English: 5,
          Science: 3,
        },
        {
          id: 4,
          name: "Ellie",
          History: 6,
          Spanish: 7,
          English: 5,
          Science: 10,
        },
        {
          id: 5,
          name: "Sarah",
          History: 10,
          Spanish: 6,
          English: 4,
          Science: 8,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="studentInfo">
    <div class="studentData">
      <h4 style="font-weight: 700" v-model="marks.name">Name:</h4>
      <input />

      <h4>Notas</h4>
      <h4 style="font-weight: 700">Subject:</h4>
      <h5>History</h5>
      <input
        type="text"
        v-model="marks.History"
        id="HistoryMark"
        name="HistoryMark"
      />
      <h5>Spanish</h5>
      <input
        type="text"
        v-model="marks.Spanish"
        id="SpanishMark"
        name="SpanishMark"
      />
      <h5>English</h5>
      <input
        type="text"
        v-model="marks.English"
        id="EnglishMark"
        name="EnglishMark"
      />
      <h5>Science</h5>
      <input
        type="text"
        v-model="marks.Science"
        id="ScienceMark"
        name="ScienceMark"
      />
    </div>

    <div class="dataTable">
      <h1>{{ title }}</h1>

      <div
        :id="marks.id"
        v-for="(marks, key) in marks"
        :key="key"
        class="marks"
      >
        <table>
          <tr>
            <th>Name</th>
            <th>History</th>
            <th>Spanish</th>
            <th>English</th>
            <th>Science</th>
          </tr>
          <tr>
            <td>{{ marks.name }}</td>
            <td>{{ marks.History }}</td>
            <td>{{ marks.Spanish }}</td>
            <td>{{ marks.English }}</td>
            <td>{{ marks.Science }}</td>
          </tr>
        </table>
      </div>
    </div>
  </div>
</template>

<style scoped>

input {
  background-color: white;
    width: 20vw;
  height: 5vh;
}
td,
th {
  border: solid grey 0.1vw;
}
table {
  border-collapse: collapse;
  width: 50vw;
}

.studentInfo{
    display:flex;
    justify-content: space-between;
}
.studentData {
  width: 30vw;
  height: auto;
  background-color: #1e2d2d;
  color: #d7fcfc;
  padding: 2vw;
  display:flex;
  flex-direction: column;
  align-items: center;
}
.dataTable {
  width: 50vw;
}
</style>

<!--
  <div
    :id="marks.id"
    v-for="(marks, key) in marks"
    :key="key"
    class="marks-trial"
  >
    <table>
      <tr>
        <th>Name</th>
        <th>History</th>
        <th><span>Spanish</span></th>
        <th>English</th>
        <th>Science</th>
      </tr>
      <tr>
        <td>{{ marks.name }}</td>
        <td>{{ marks.History }}</td>
        <td>{{ marks.Spanish }}</td>
        <td>{{ marks.English }}</td>
        <td>{{ marks.Science }}</td>
      </tr>
    </table>
  </div>
  -->
