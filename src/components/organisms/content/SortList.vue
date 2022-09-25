<template>
  <div>
    <div class="d-flex">
      <span class="text-nowrap sort-text me-3">Sort by : </span>
      <div class="sort-listing position-relative">
        <SortListing value="Default" :status="true" />
        <SortListing value="Popularity" />
        <SortListing value="Price high" />
        <SortListing value="Price low" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import SortListing from "../../molecules/sortListing/SortListing.vue";

@Options({
  components: { SortListing },
})
export default class SortList extends Vue {}
</script>

<style lang="scss">
.sort-text {
  font-size: 20px;
  color: #707070;
}

.sort-listing::after {
  content: "";
  position: absolute;
  right: 0;
  bottom: 0;
  left: 80%;
  top: 0;
  background: linear-gradient(90deg, transparent 0%, #f6f6f6 30%);
}
</style>
