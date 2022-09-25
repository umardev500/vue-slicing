<template>
  <div class="ps-lg-4 mt-5 mt-lg-0">
    <CollectionList />
    <ShopAllList />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import CollectionList from "./CollectionList.vue";
import ShopAllList from "./ShopAllList.vue";

@Options({
  components: {
    CollectionList,
    ShopAllList,
  },
})
export default class Content extends Vue {}
</script>
