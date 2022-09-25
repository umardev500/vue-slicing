<template>
  <div>
    <Navbar />
    <Banner />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navbar from "@/components/molecules/navbar/Navbar.vue";
import Banner from "../banner/Banner.vue";

@Options({
  components: {
    Navbar,
    Banner,
  },
})
export default class Header extends Vue {}
</script>

<style lang="scss"></style>
