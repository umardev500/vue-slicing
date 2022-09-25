<template>
  <div class="bg-white rounded mb-4 overflow-hidden" role="button">
    <div class="thumb-wrapper position-relative">
      <img class="w-100" src="../../../../assets/thumbs/1.png" alt="thumb" />
    </div>
    <div class="px-3 py-3">
      <div>
        <span class="d-flex p-0 lh-1 product-category">Skincare</span>
        <span class="d-flex p-0 product-name fw-bold">Product Name</span>
      </div>
      <div class="mt-2 d-flex">
        <span class="product-price-cut">798 HKD</span>
        <span class="product-price-cut-percentage">50% off</span>
      </div>
      <div class="d-flex align-items-end">
        <span class="product-price fw-bold lh-1">399</span>
        <span class="product-price-currency">HKD</span>
      </div>
      <div class="d-flex flex-fill flex-wrap mt-3">
        <span class="badge text-white product-badge">Discount</span>
        <span class="badge text-white product-badge">Free Shipping</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.thumb-wrapper::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: linear-gradient(180deg, #252525 0%, rgba(37, 37, 37, 0) 38.5%);
}
.product-name {
  font-size: 24px;
  color: #333;
}

.product-category {
  color: #333;
  opacity: 0.5;
}

.product-price-cut {
  text-decoration: line-through;
  margin-right: 6px;
  color: $blackColor;
  opacity: 0.5;
  font-size: 15px;
}

.product-price-cut-percentage {
  color: $pinkColor;
  opacity: 0.5;
  font-size: 15px;
}

.product-price {
  color: $pinkColor;
  font-size: 45px;
  margin-right: 6px;
}

.product-price-currency {
  color: $blackColor;
  font-size: 15px;
  font-weight: 500;
}

.product-badge {
  background-color: $pinkColor;
  margin-right: 5px;
  margin-bottom: 5px;
}
</style>
