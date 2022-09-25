<template>
  <div class="d-flex justify-content-center align-items-center mt-3">
    <div>
      <i class="fa-solid fa-caret-left prev prev-next font-size"></i>
    </div>
    <PaginationListing value="1" />
    <PaginationListing value="2" />
    <PaginationListing value="3" />
    <PaginationListing value="..." />
    <PaginationListing value="20" />
    <div>
      <i class="fa-solid fa-caret-right prev-next font-size"></i>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import PaginationListing from "@/components/molecules/paginationListing/PaginationListing.vue";

export default defineComponent({
  name: "Pagination",
  components: { PaginationListing },
});
</script>

<style lang="scss">
.prev-next {
  font-size: 30px;
  color: $appColorPrimary;
}

.prev {
  margin-right: 40px;
}
</style>
