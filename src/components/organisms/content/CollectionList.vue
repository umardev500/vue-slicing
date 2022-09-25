<template>
  <div>
    <div class="d-flex align-items-center justify-content-between mb-4">
      <ContentLabel class="d-flex" value="Collections" />
      <div class="collection-seeall" role="button">
        <span>See all</span>
        <i class="fa-solid fa-angle-right ms-2"></i>
      </div>
    </div>
    <div class="d-flex collections">
      <!-- loop here -->
      <CollectionListing role="button" value="summer" />
      <CollectionListing role="button" value="spring" />
      <CollectionListing role="button" value="winter" />
      <!-- end -->
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import CollectionListing from "@/components/molecules/collectionListing/CollectionListing.vue";
import ContentLabel from "@/components/atoms/label/ContentLabel.vue";

@Options({
  components: { CollectionListing, ContentLabel },
})
export default class CollectionList extends Vue {}
</script>

<style lang="scss">
.collections > :not(:first-child) {
  margin-left: 10px;
}

.collection-seeall {
  color: $appColorPrimary;
  overflow: 0.5;
}

@media (min-width: 992px) {
  .collections > :not(:first-child) {
    margin-left: 20px;
  }
}
</style>
