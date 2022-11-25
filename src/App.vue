<script setup>
import TableAction from "./components/TableAction.vue";
import TableHeader from "./components/TableHeader.vue";
import TableBody from "./components/TableBody.vue";
import TableFooter from "./components/TableFooter.vue";
</script>

<template>
  <div class="table-basic">
    <table-action></table-action>
    <table class="table">
      <table-header></table-header>
      <table-body></table-body>
    </table>
    <table-footer></table-footer>
  </div>
</template>

<style scoped>
.table-basic .table {
  width: 100%;
  border: none;
  border-collapse: collapse;
}
</style>
