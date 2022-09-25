<template>
  <div class="mt-5 row">
    <div class="col-lg-4">
      <ProductListing />
    </div>
    <div class="col-lg-4">
      <ProductListing />
    </div>
    <div class="col-lg-4">
      <ProductListing />
    </div>
    <div class="col-lg-4">
      <ProductListing />
    </div>
    <div class="col-lg-4">
      <ProductListing />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ProductListing from "@/components/molecules/productListing/ProductListing.vue";

export default defineComponent({
  name: "ProductList",
  components: { ProductListing },
});
</script>
