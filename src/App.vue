<template>
  <div class="table-basic">
    <table-action></table-action>
    <table class="table">
      <table-header></table-header>
      <table-body
        v-if="data"
        :results="data"></table-body>
    </table>
    <table-footer></table-footer>
  </div>
</template>

<script setup>
import TableAction from "./components/TableAction.vue";
import TableHeader from "./components/TableHeader.vue";
import TableBody from "./components/TableBody.vue";
import TableFooter from "./components/TableFooter.vue";
import axios from "axios";
import { ref } from "vue";

let data = ref();

const fetchData = async function () {
  const res = await axios.get(
    "https://randomapi.com/api/6de6abfedb24f889e0b5f675edc50deb"
  );
  data.value = res.data;
};

fetchData();
</script>

<style scoped>
.table-basic .table {
  width: 100%;
  border: none;
  border-collapse: collapse;
}
</style>
