<script setup></script>

<template>
  <div class="select-mediam">
    <label>Show</label>
    <select>
      <option
        value="10"
        selected>
        10
      </option>
      <option value="20">20</option>
      <option value="50">50</option>
      <option value="100">100</option>
      <option value="200">200</option>
    </select>
  </div>
</template>

<style scoped>
.select-mediam {
  display: flex;
  align-items: center;
  gap: 20px;
}

.select-mediam label {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  color: #6e6b7b;
}

.select-mediam select {
  background: #ffffff;
  border-radius: 6px;
  border: 1px solid #d8d6de;
  padding: 10px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 24px;
  color: #b9b9c3;
}
</style>
