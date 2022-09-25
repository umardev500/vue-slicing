<template>
  <Header />
  <div class="container">
    <div class="row">
      <div class="col-lg-4">
        <Sidebar />
      </div>
      <div class="col-lg-8">hallo</div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import { Header } from "@/components/organisms/header";
import Banner from "@/components/organisms/banner/Banner.vue";
import { Sidebar } from "@/components/organisms/sidebar";

@Options({
  components: {
    Header,
    Banner,
    Sidebar,
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
