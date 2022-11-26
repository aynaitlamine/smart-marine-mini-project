<script setup>
import { computed, defineProps, onMounted, ref } from "vue";
import moment from "moment";
const empolyee = ref({});

const props = defineProps({
  data: {
    type: Object,
  },
});

onMounted(() => {
  const { data } = props;
  empolyee.value = data;
});

const createdAt = computed(() => {
  return moment(new Date(empolyee.value.created))
    .format("DD/MM/YYYY")
    .replace(/\//g, ".");
});
</script>

<template>
  <tr class="table-row">
    <td>{{ empolyee.first }}</td>
    <td>{{ empolyee.last }}</td>
    <td>{{ empolyee.address }}</td>
    <td>{{ empolyee.email }}</td>
    <td>{{ createdAt }}</td>
    <td>{{ empolyee.balance }}</td>
  </tr>
</template>

<style scoped>
.table-row {
  background: #ffffff;
  padding: 20px;
}

.table-row > td {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  color: #6e6b7b;
  border-bottom: 2px solid #f3f2f7;
  border-top: 2px solid #f3f2f7;
  text-align: left;
  padding: 20px;
}

.table-row td:nth-child(5) {
  font-size: 12px;
  line-height: 15px;
  color: #000000;
}

.table-row td:nth-child(6) {
  font-size: 12px;
  line-height: 15px;

  color: #000000;
}
</style>
