<template>
  <div class="ps-lg-4 mt-5 mt-lg-0">
    <CollectionList />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import CollectionList from "./CollectionList.vue";

@Options({
  components: {
    CollectionList,
  },
})
export default class Content extends Vue {}
</script>
