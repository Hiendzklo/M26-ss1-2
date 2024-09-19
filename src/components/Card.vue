<template>
  <div class="card">
    <div class="card-image">
      <span>Image</span>
    </div>
    <div class="card-content">
      <h3>Title</h3>
      <button class="add-to-card-btn">Add to card</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
};
</script>

<style scoped>
.card {
  width: 200px;
  border: 1px solid #ddd;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  text-align: center;
  font-family: Arial, sans-serif;
  background-color: #fff;
}

.card-image {
  background-color: #888;
  height: 150px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 18px;
}

.card-content {
  padding: 10px;
}

h3 {
  font-size: 16px;
  margin: 10px 0;
}

.add-to-card-btn {
  border: 1px solid #ccc;
  background-color: #f9f9f9;
  padding: 5px 10px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.add-to-card-btn:hover {
  background-color: #eee;
}
</style>
