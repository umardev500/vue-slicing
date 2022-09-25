<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-transparent">
    <div class="container-fluid header-container">
      <a class="navbar-brand fw-bold" href="#">NOGONOBUDDY</a>

      <NavbarRight class="d-lg-none" />

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- collapsable menu -->
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <!-- nav items -->
          <li v-for="item in items" class="nav-item">
            <a
              :class="['nav-link text-uppercase', item.status && 'active']"
              aria-current="page"
              href="#"
              >{{ item.name }}</a
            >
          </li>
          <!-- end of nav items -->
        </ul>
      </div>
      <!-- end of collapsable menu -->

      <!-- right menu -->
      <NavbarRight class="d-none d-lg-flex ms-lg-4" />

      <!-- end of right menu -->
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { navigation } from "./navigation.knob";
import NavbarRight from "./NavbarRight.vue";

export default defineComponent({
  name: "Navbar",
  data() {
    return {
      items: navigation,
    };
  },
  components: { NavbarRight },
});
</script>

<style lang="scss">
.navbar {
  position: absolute !important;
  left: 0;
  right: 0;
  z-index: 1050;
  top: 20px;
}

.nav-link {
  font-family: Abel;
  font-weight: 700 !important;
}

@media (min-width: 992px) {
  .header-container {
    padding-left: 60px !important;
    padding-right: 60px !important;
  }

  .navbar .nav-link {
    padding-left: 12.5px !important;
    padding-right: 12.5px !important;
  }

  .navbar-brand {
    letter-spacing: 21px;
    font-size: 24px;
  }

  .nav-link.active {
    position: relative;
  }

  .nav-link.active::after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 25%;
    right: 25%;
    background: white;
    height: 2.5px;
    border-radius: 1.5px;
  }
}
</style>
