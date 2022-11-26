<template>
  <tbody class="table-body">
    <table-row
      v-for="(empolyee, index) in empolyees"
      :key="index"
      :data="empolyee"></table-row>
  </tbody>
</template>

<script setup>
import TableRow from "./TableRow.vue";
import { defineProps, onMounted, ref } from "vue";

const empolyees = ref([]);

const props = defineProps({
  results: {
    type: Object,
  },
});

onMounted(() => {
  const { results } = props;
  empolyees.value = results.results[0];
});
</script>

<style scoped></style>
