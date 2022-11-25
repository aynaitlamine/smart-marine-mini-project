<script setup>
import TablePagination from "./TablePagination.vue";
</script>

<template>
  <div class="table-footer">
    <div class="result">Showing 1 to 7 of 100 entries</div>
    <table-pagination></table-pagination>
  </div>
</template>

<style scoped>
.table-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 32px;
}

.table-footer .result {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  color: #b9b9c3;
}
</style>
