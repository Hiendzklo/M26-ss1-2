<template>
  <div id="app">
    <h1>Danh sách khóa học</h1>
    <ListCourse />
    
    <h1>Màu sắc của các khối</h1>
    <div class="color-boxes">
      <ColorBox color="red" />
      <ColorBox color="blue" />
      <ColorBox color="green" />
    </div>
    
    <h1>Thẻ sản phẩm</h1>
    <div class="card-section">
      <Card />
    </div>

    <h1>Danh sách kết quả tính toán</h1>
    <div class="calculation-section">
      <Calculation />
    </div>
  </div>
</template>

<script>
import ListCourse from './components/ListCourse.vue'
import ColorBox from './components/ColorBox.vue'
import Card from './components/Card.vue'
import Calculation from './components/Calculation.vue'

export default {
  components: {
    ListCourse,
    ColorBox,
    Card,
    Calculation
  }
}
</script>

<style>
#app {
  text-align: center;
  margin-top: 20px;
}

.color-boxes {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.card-section {
  margin-top: 20px;
}

.calculation-section {
  margin-top: 20px;
}
</style>
