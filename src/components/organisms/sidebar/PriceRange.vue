<template>
  <div class="mt-4">
    <Label class="fw-bold d-inline-flex mb-3" value="Price range" />
    <div class="range-container d-flex flex-column position-relative mt-3">
      <input
        type="range"
        class="range form-range w-100"
        value="30"
        max="1000"
        @input="slideMin($event)"
      />
      <input
        type="range"
        class="range range-max form-range w-100"
        value="1000"
        max="1000"
        @input="slide($event)"
      />
      <span
        class="range-value range-value-max fw-bold text-nowrap"
        :style="[{ left: 0 + '%' }]"
        >{{ rangeValueMin }} HKD</span
      >
      <span
        class="range-value range-value-min fw-bold text-nowrap"
        :style="[{ right: 0 + '%' }]"
        >{{ rangeValueMax }} HKD</span
      >
    </div>
  </div>
</template>

<script lang="ts">
import Label from "@/components/atoms/label/Label.vue";
import { defineComponent } from "vue";

let minGap = 5;

export default defineComponent({
  components: { Label },
  data: () => {
    return {
      rangeValueMin: 30,
      rangeValueMax: 1000,
    };
  },
  methods: {
    slide: function (event: any) {
      var val = event.target.valueAsNumber;

      var result = val - this.rangeValueMin;
      if (result <= minGap) {
        event.target.value = this.rangeValueMin + minGap;
        this.rangeValueMax = this.rangeValueMin;
      } else {
        this.rangeValueMax = val;
      }
    },
    slideMin: function (event: any) {
      var val = event.target.valueAsNumber;

      var result = this.rangeValueMax - val;
      if (result <= minGap) {
        event.target.value = this.rangeValueMax - minGap;
        this.rangeValueMin = this.rangeValueMax;
      } else {
        this.rangeValueMin = val;
      }
    },
  },
});
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

.range-value {
  font-size: 20px;
  position: absolute;
  color: #707070;
  opacity: 0.8;
  top: 25px;
}

.range-value-max {
}

.range-value-min {
}
</style>
