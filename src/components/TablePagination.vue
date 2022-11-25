<script setup>
import IconArrowLeft from "./Icons/IconArrowLeft.vue";
import IconArrowRight from "./Icons/IconArrowRight.vue";
</script>

<template>
  <div class="table-pagination">
    <a
      class="prev"
      href="#">
      <icon-arrow-right></icon-arrow-right>
    </a>
    <div class="page-items">
      <a
        class="page-link"
        href="#"
        >1</a
      >
      <a
        class="page-link"
        href="#"
        >2</a
      >
      <a
        class="page-link"
        href="#"
        >3</a
      >
      <a
        class="page-link active-link"
        href="#"
        >4</a
      >
      <a
        class="page-link"
        href="#"
        >5</a
      >
      <a
        class="page-link"
        href="#"
        >6</a
      >

      <a
        class="page-link"
        href="#"
        >7</a
      >
    </div>
    <a
      class="next"
      href="#">
      <icon-arrow-left></icon-arrow-left>
    </a>
  </div>
</template>

<style scoped>
.table-pagination {
  display: flex;
  align-items: center;
  gap: 10px;
}
.prev,
.next {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 20px;
  background: #f3f2f7;
  border-radius: 29px;
  padding: 5px;
  text-decoration: none;
}
.page-items {
  display: flex;
  align-items: center;
  background: #f3f2f7;
  border-radius: 16px;
  gap: 5px;
  padding: 0px 5px;
}

.page-items .page-link {
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  color: #6e6b7b;
  text-decoration: none;
  padding: 5px;
}

.page-items .active-link {
  width: 20px;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  color: #ffffff;
  background: #0b308e;
  border-radius: 29px;
}
</style>
