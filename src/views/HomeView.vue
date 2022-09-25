<template>
  <Header />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import { Header } from "@/components/organisms/header";
import Banner from "@/components/organisms/banner/Banner.vue";

@Options({
  components: {
    Header,
    Banner,
  },
})
export default class HomeView extends Vue {}
</script>

<style>
.app-container {
  background-color: #f6f6f6;
  padding-top: 50px;
  padding-bottom: 50px;
  min-height: 100vh;
}
</style>
