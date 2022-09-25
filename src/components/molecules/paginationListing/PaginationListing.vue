<template>
  <div
    class="pagination-item d-inline-flex fw-bold rounded-pill align-items-center justify-content-center"
  >
    {{ value }}
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "PaginationListing",
  components: {},
  props: {
    value: { type: String },
  },
});
</script>

<style lang="scss">
.pagination-item {
  border: 2px solid $appColorPrimary;
  width: 50px;
  height: 50px;
  color: $appColorPrimary;
  font-size: 18px;
  margin-right: 40px;
}
</style>
