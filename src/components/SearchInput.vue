<script setup></script>

<template>
  <div class="search-input">
    <label>Search</label>
    <input placeholder="Search" />
  </div>
</template>

<style scoped>
.search-input {
  display: flex;
  align-items: center;
  gap: 20px;
}

.search-input label {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  color: #6e6b7b;
}
.search-input input {
  background: #ffffff;
  border-radius: 5px;
  border: 1px solid #d8d6de;
  padding: 10px;
}

.search-input input::placeholder {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 24px;
  color: #b9b9c3;
}
</style>
