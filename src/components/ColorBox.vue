<template>
  <div class="box-container">
    <div class="box" :style="{ backgroundColor: color }">
      <span>Box</span>
    </div>
    <div class="color-label">
      <span>{{ color }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "ColorBox",
  props: {
    color: {
      type: String,
      required: true,
      validator(value) {
        // Chỉ cho phép các màu 'red', 'blue', hoặc 'green'
        return ['red', 'blue', 'green'].includes(value);
      }
    }
  }
};
</script>

<style scoped>
.box-container {
  display: inline-block;
  text-align: center;
  margin: 10px;
}

.box {
  width: 200px;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 20px;
  border-radius: 5px;
}

.color-label {
  margin-top: 10px;
}

.color-label span {
  background-color: #eee;
  padding: 5px 10px;
  border-radius: 5px;
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.2);
}

.box-container:after {
  content: '';
  display: block;
  width: 0;
  height: 0;
  margin: 0 auto;
  border-left: 10px solid transparent;
  border-right: 10px solid transparent;
  border-top: 10px solid #ddd;
}
</style>
