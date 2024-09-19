<template>
  <div class="calculation">
    <h1>Danh sách kết quả</h1>
    <ul>
      <li>10 + 10 = {{ add(10, 10) }}</li>
      <li>10 - 10 = {{ subtract(10, 10) }}</li>
      <li>10 * 10 = {{ multiply(10, 10) }}</li>
      <li>10 / 10 = {{ divide(10, 10) }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Calculation",
  methods: {
    add(a, b) {
      return a + b;
    },
    subtract(a, b) {
      return a - b;
    },
    multiply(a, b) {
      return a * b;
    },
    divide(a, b) {
      return a / b;
    }
  }
};
</script>

<style scoped>
.calculation {
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

ul {
  list-style-type: disc;
  padding-left: 20px;
}

li {
  font-size: 16px;
  margin: 5px 0;
}
</style>
