<template>
  <div>
    <span>{{ value }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "CollectionListing",
  props: {
    value: { type: String },
  },
});
</script>
