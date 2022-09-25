<template>
  <ul class="navbar-nav me-4 ms-auto flex-row">
    <li class="nav-item dropdown position-relative">
      <a
        class="nav-link language-dropdown-link px-2 py-1 rounded"
        href="#"
        role="button"
        data-bs-toggle="dropdown"
        aria-expanded="false"
      >
        <i class="fa-solid fa-earth-americas me-1"></i>
        <i class="fa-solid fa-angle-down ms-2"></i>
      </a>
      <ul
        class="dropdown-menu position-absolute bg-transparent language-dropdown"
        style="right: 0; left: unset"
      >
        <li><a class="dropdown-item active" href="#">English</a></li>
        <li><a class="dropdown-item" href="#">中文</a></li>
      </ul>
    </li>
    <li class="nav-item">
      <a
        class="nav-link px-2 py-1 ms-3 d-flex"
        href="#"
        role="button"
        data-bs-toggle="dropdown"
        aria-expanded="false"
      >
        <i class="fa-solid fa-cart-arrow-down fs-4 text-white"></i>
      </a>
    </li>
  </ul>
</template>

<style>
.language-dropdown-link {
  border: 2px solid white;
}

.language-dropdown {
  border-color: white !important;
  border-width: 1.5px !important;
}

.language-dropdown .dropdown-item {
  color: white !important;
}

.language-dropdown .dropdown-item.active {
  color: #05c4c4 !important;
  background-color: transparent !important;
}
.language-dropdown .dropdown-item:hover {
  background-color: unset !important;
  color: #05c4c4 !important;
}
</style>
