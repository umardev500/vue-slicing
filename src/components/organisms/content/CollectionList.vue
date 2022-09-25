<template>
  <div>
    <ContentLabel value="Collections" />
    <CollectionListing />
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
