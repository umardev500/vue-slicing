<template>
  <div
    role="button"
    :class="[
      'pagination-item d-inline-flex fw-bold rounded-pill align-items-center justify-content-center',
      more && 'more-item',
    ]"
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
    more: { type: Boolean },
  },
});
</script>

<style lang="scss">
.pagination-item {
  border: 2px solid $appColorPrimary;
  width: 50px;
  height: 50px;
  color: $appColorPrimary;
  opacity: 0.5;
  font-size: 18px;
  margin-right: 40px;
}

.more-item {
  border-color: transparent !important;
}
</style>
