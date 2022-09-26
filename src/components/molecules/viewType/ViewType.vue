<template>
  <div>
    <div class="d-flex align-items-center">
      <span class="text-nowrap sort-text me-3 text-nowrap">View : </span>
      <div class="dropdown">
        <button
          class="btn btn-secondary d-flex align-items-center card-view-button px-2 py-1"
          type="button"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          <span class="card-view-text">Card</span>
          <i class="fa-solid fa-angle-down card-view-icon ms-2"></i>
        </button>
        <!-- <ul class="dropdown-menu dropdown-menu-view-type">
          <li><a class="dropdown-item" href="#">Action</a></li>
          <li><a class="dropdown-item" href="#">Another action</a></li>
          <li><a class="dropdown-item" href="#">Something else here</a></li>
        </ul> -->
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.view-text {
  font-size: 20px;
  color: #707070;
}

.card-view-button {
  background-color: transparent !important;
  border: 2px solid rgba(196, 196, 196, 0.5) !important;
  border-radius: 10px !important;
  padding: 0 !important;
}

.card-view-text,
.card-view-icon {
  color: #707070;
  opacity: 0.5;
}

.card-view-icon {
  font-size: 14px;
}

.card-view-text {
  margin-bottom: -2px;
}

.dropdown-menu-view-type {
  right: 0 !important;
  left: unset !important;
}
</style>
