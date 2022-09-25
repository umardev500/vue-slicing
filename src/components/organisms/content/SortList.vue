<template>
  <div>
    <div>
      <span class="text-nowrap sort-text me-3">Sort by : </span>
      <SortListing value="Default" :status="true" />
      <SortListing value="Popularity" />
      <SortListing value="Price high" />
      <SortListing value="Price low" />
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
</style>
