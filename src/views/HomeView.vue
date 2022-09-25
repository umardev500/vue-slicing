<template>
  <Header />
  <div class="app-container pt-lg-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <Sidebar />
        </div>
        <div class="col-lg-8">
          <Content />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import { Header } from "@/components/organisms/header";
import Banner from "@/components/organisms/banner/Banner.vue";
import { Sidebar } from "@/components/organisms/sidebar";
import Content from "@/components/organisms/content/Content.vue";

@Options({
  components: {
    Header,
    Banner,
    Sidebar,
    Content,
  },
})
export default class HomeView extends Vue {}
</script>

<style>
.app-container {
  padding-bottom: 50px;
  min-height: 100vh;
}

@media (min-width: 992px) {
  .app-container {
    padding-left: 75px;
    padding-right: 75px;
  }
}
</style>
