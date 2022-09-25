<template>
  <div>
    <Label class="fw-bold d-inline-flex mb-3" value="Categories" />
    <CategoryListing value="All (1080)" />
    <CategoryListing value="Arts & Crafts (38)" />
    <CategoryListing value="Fitness & Sports (469)" />
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
