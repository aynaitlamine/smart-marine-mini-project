<script setup>
import IconChevronUp from "./Icons/IconChevronUp.vue";
import IconChevronDown from "./Icons/IconChevronDown.vue";
</script>

<template>
  <tbody class="table-header">
    <tr>
      <th>
        <div class="header-name">
          first name
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
      <th>
        <div class="header-name">
          last name
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
      <th>
        <div class="header-name">
          address
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
      <th>
        <div class="header-name">
          email
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
      <th>
        <div class="header-name">
          created at
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
      <th>
        <div class="header-name">
          balance
          <div class="header-filter">
            <button>
              <icon-chevron-up></icon-chevron-up>
            </button>

            <button>
              <icon-chevron-down></icon-chevron-down>
            </button>
          </div>
        </div>
      </th>
    </tr>
  </tbody>
</template>

<style scoped>
.table-header {
  border: none;
  background: #f3f2f7 !important;
}

.table-header th {
  background: #f3f2f7 !important;
  border: none;
  padding: 20px;
  font-weight: 600;
  font-size: 12px;
  line-height: 15px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #5e5873;
  border-bottom: 2px solid #f3f2f7;
  text-align: left;
}

.table-header .header-name {
  display: flex;
  align-items: center;
  gap: 5px;
}

.table-header .header-filter {
  display: flex;
  flex-direction: column;
}
.table-header .header-filter button {
  border: none;
  background: transparent;
}
</style>
