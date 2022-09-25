<template>
  <div class="mt-5">
    <!-- Heading -->
    <div class="d-flex align-items-center justify-content-between mb-4">
      <ContentLabel class="d-flex" value="shop all" />
      <div class="collection-seeall" role="button">
        <span>See all</span>
        <i class="fa-solid fa-angle-right ms-2"></i>
      </div>
    </div>

    <div class="d-flex justify-content-between">
      <!-- Sort list -->
      <SortList />

      <!-- View type -->
      <ViewType />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import ContentLabel from "@/components/atoms/label/ContentLabel.vue";
import SortList from "./SortList.vue";
import ViewType from "@/components/molecules/viewType/ViewType.vue";

@Options({
  components: { ContentLabel, SortList, ViewType },
})
export default class ShopAllList extends Vue {}
</script>
