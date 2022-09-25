<template>
  <Label :value="value" class="fw-bold content-label text-uppercase" />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Label from "./Label.vue";

export default defineComponent({
  name: "ContentLabel",
  props: {
    value: { type: String },
  },
  components: { Label },
});
</script>

<style lang="scss">
.content-label {
  font-size: 24px;
  color: #324158;
}
</style>
