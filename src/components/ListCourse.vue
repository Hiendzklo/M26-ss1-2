<template>
  <div class="list-course">
    <h1>Danh sách khóa học</h1>
    <ol>
      <li v-for="(course, index) in courses" :key="index">
        {{ course }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  name: "ListCourse",
  data() {
    return {
      courses: ["HTML", "CSS", "JavaScript", "ReactJS"]
    };
  }
};
</script>

<style scoped>
.list-course {
  width: 200px;
  border: 1px solid #ddd;
  padding: 10px;
  border-radius: 5px;
  font-family: Arial, sans-serif;
}

h1 {
  font-size: 18px;
  text-align: center;
  margin-bottom: 10px;
  font-weight: bold;
}

ol {
  list-style-type: decimal;
  padding-left: 20px;
}

li {
  font-size: 16px;
  margin: 5px 0;
}
</style>
