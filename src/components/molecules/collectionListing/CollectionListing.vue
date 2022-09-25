<template>
  <div
    class="collection-card w-100 rounded py-2 px-3 d-flex align-items-center justify-content-center"
  >
    <span class="collection-text text-uppercase text-white fw-bold">{{
      value
    }}</span>
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

<style lang="scss">
.collection-card {
  background-color: #9e9e9e;
}

.collection-text {
  font-size: 20px;
}
@media (min-width: 992px) {
  .collection-text {
    padding-top: 40px;
    padding-bottom: 40px;
    font-size: 30px;
  }
}
</style>
