<template>
  <div class="mt-4">
    <Label class="fw-bold d-inline-flex mb-3" value="Price range" />
    <div class="range-container d-flex flex-column position-relative mt-3">
      <input type="range" class="range form-range w-100" value="30" />
      <input
        type="range"
        class="range range-max form-range w-100"
        value="100"
      />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Label from "@/components/atoms/label/Label.vue";

@Options({
  components: {
    Label,
  },
})
export default class PriceRange extends Vue {}
</script>

<style>
.range {
  appearance: none;
  height: unset !important;
}

.range:focus {
  outline: 1;
}

.range::-webkit-slider-thumb {
  box-shadow: inset 1px 1px 2px rgba(0, 0, 0, 0.15) !important;
  background-color: #ffca40 !important;
  border: 2px solid white !important;
  width: 24px !important;
  height: 24px !important;
  margin-top: -9px !important;
  box-shadow: 2px 2px 3px rgba(0, 0, 0, 0.15);
}

.range-max {
  position: absolute;
  top: 20px;
  padding: 0 !important;
}

.range-max::-webkit-slider-thumb {
  margin-top: -29px !important;
  z-index: 1030;
}

.range-max::-webkit-slider-runnable-track {
  background-color: transparent !important;
}
</style>
