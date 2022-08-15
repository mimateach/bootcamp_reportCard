<!-- eslint-disable vue/require-v-for-key -->
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
  <div>
    <h4>Nombre</h4>
<input/>

<!--<select>
    <option v-model="marks.History" id="history">History</option>
    <option>Spanish</option>
    <option>English</option>
    <option>Science</option>
</select>-->
    <h4>Nota</h4>
    <h4>Subject</h4>
    <h6>History</h6>
<input type="text" v-model="marks.History" id="HistoryMark" name="HistoryMark">
    <h6>Spanish</h6>
<input type="text" v-model="marks.Spanish" id="SpanishMark" name="SpanishMark">
    <h6>English</h6>
<input type="text" v-model="marks.English" id="EnglishMark" name="EnglishMark">
    <h6>Science</h6>
<input type="text" v-model="marks.Science" id="ScienceMark" name="ScienceMark">

</div>
</template>

<style scoped>
input {
  background-color: white;
  width: 40vw;
  height: 5vh;
}
</style>
