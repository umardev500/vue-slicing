<template>
  <div class="hashtag-card rounded-pill px-2 py-1 d-inline-flex">
    <span class="hashtag-text text-nowrap">{{ value }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HashtagListing",
  props: {
    value: { type: String },
  },
});
</script>

<style lang="scss">
.hashtag-card {
  border: 2px solid;
  border-color: #e1e1e1;
  margin-right: 10px;
  margin-bottom: 10px;
  background-color: #e1e1e1;
}

.hashtag-text {
  color: #707070;
  opacity: 0.8;
  font-size: 15px;
}
</style>
