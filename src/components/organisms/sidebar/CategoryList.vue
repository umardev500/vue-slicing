<template>
  <div>
    <Label class="fw-bold d-inline-flex mb-3" value="Categories" />
    <CategoryListing value="All (1080)" />
    <CategoryListing value="Arts & Crafts (38)" />
    <CategoryListing value="Fitness & Sports (469)" />
    <div class="ms-3">
      <span class="show-all-text fw-bold">Show all</span>
      <i class="fa-solid fa-angle-down ms-2 show-all-caret"></i>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import CategoryListing from "@/components/molecules/categoryListing/CategoryListing.vue";
import Label from "@/components/atoms/label/Label.vue";

@Options({
  components: {
    CategoryListing,
    Label,
  },
})
export default class CategoryList extends Vue {}
</script>

<style lang="scss">
.show-all-text {
  color: $appColorPrimary;
  opacity: 0.8;
}

.show-all-caret {
  color: $appColorPrimary;
}
</style>
