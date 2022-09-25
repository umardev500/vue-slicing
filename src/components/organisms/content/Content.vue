<template>
  <div class="ps-lg-4 mt-5 mt-lg-0">
    <CollectionList />
    <ShopAllList />
    <Search />
    <ProductList />
    <Pagination />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import CollectionList from "./CollectionList.vue";
import ShopAllList from "./ShopAllList.vue";
import Search from "./Search.vue";
import ProductList from "../productList/ProductList.vue";
import Pagination from "../pagination/Pagination.vue";

@Options({
  components: {
    CollectionList,
    ShopAllList,
    Search,
    ProductList,
    Pagination,
  },
})
export default class Content extends Vue {}
</script>
