<template>
  <span class="label">{{ value }}</span>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Label",
  props: {
    value: {
      type: String,
    },
  },
});
</script>

<style lang="scss">
.label {
  color: #707070;
  font-size: 20px;
}
</style>
