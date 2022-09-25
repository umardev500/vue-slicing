<template>
  <div>
    <div class="sidebar-inner rounded">
      <CategoryList />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Label from "@/components/atoms/label/Label.vue";
import CategoryList from "./CategoryList.vue";

@Options({
  components: { Label, CategoryList },
})
export default class Sidebar extends Vue {}
</script>

<style lang="scss">
.sidebar-inner {
  background-color: white;
  padding-left: 40px;
  padding-right: 40px;
  padding-top: 30px;
  padding-bottom: 50px;
}
</style>
