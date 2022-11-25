<script setup>
import SelectMediam from "./SelectMediam.vue";
import SearchInput from "./SearchInput.vue";
</script>

<template>
  <div class="table-action">
    <select-mediam></select-mediam>
    <search-input></search-input>
  </div>
</template>

<style scoped>
.table-action {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 32px;
}
</style>
