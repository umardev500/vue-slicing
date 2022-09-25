<template>
  <div class="ms-3 d-flex align-items-center mb-3">
    <input type="checkbox" class="form-check-input category-check" />
    <span class="category-text">{{ value }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "CategoryListing",
  props: {
    value: { type: String },
  },
});
</script>

<style lang="scss">
.category-check {
  width: 24px !important;
  height: 24px !important;
  border-color: $borderColor !important;
  border-width: 2px !important;
  margin-top: 0 !important;
  margin-right: 8px !important;
}

.category-text {
  color: #707070;
  opacity: 0.8;
}
</style>
