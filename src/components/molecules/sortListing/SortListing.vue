<template>
  <HashtagListing
    role="button"
    :value="value"
    :class="['px-3 hashtag-active sort-item', status && 'active']"
  />
</template>

<script lang="ts">
import HashtagListing from "@/components/molecules/hashtagListing/HashtagListing.vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "SortListing",
  props: {
    value: { type: String },
    status: { type: Boolean },
  },
  components: { HashtagListing },
});
</script>

<style lang="scss">
.sort-item {
  background-color: transparent;
}

.sort-item.active {
  background-color: $appColorPrimary;
  border-color: $appColorPrimary;
}

.sort-item > span {
  color: #707070;
  opacity: 0.5;
  font-size: 16px;
  font-weight: 500;
}
.sort-item.active > span {
  color: white;
  opacity: unset;
}
</style>
