<template>
  <div>
    <Label class="fw-bold d-inline-flex mb-3 mt-4" value="Hashtags" />
    <div>
      <HashtagListing value="Skincare" />
      <HashtagListing value="Coffee" />
      <HashtagListing value="Beverages" />
      <HashtagListing value="Tragicomedies" />
      <HashtagListing value="Literature Review" />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Label from "@/components/atoms/label/Label.vue";
import HashtagListing from "@/components/molecules/hashtagListing/HashtagListing.vue";

@Options({
  components: {
    Label,
    HashtagListing,
  },
})
export default class HashtagList extends Vue {}
</script>
