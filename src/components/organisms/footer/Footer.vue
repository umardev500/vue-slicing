<template>
  <div class="mt-5">
    <footer class="footer">
      <div class="container">
        <div class="row">
          <!-- left footer -->
          <div class="col-lg-8">
            <!-- brand -->
            <span class="footer-brand-name d-flex text-white"
              >STORE NAME LTD.</span
            >
            <!-- end -->

            <!-- social -->
            <div class="mt-3">
              <a href="fo" class="text-white footer-social">
                <i class="fa-brands fa-instagram"></i>
              </a>
              <a href="fo" class="text-white footer-social">
                <i class="fa-brands fa-instagram"></i>
              </a>
              <a href="fo" class="text-white footer-social">
                <i class="fa-brands fa-instagram"></i>
              </a>
              <a href="fo" class="text-white footer-social">
                <i class="fa-brands fa-instagram"></i>
              </a>
            </div>
            <!-- end -->
          </div>

          <!-- right footer -->
          <div class="col-lg-4">
            <span class="text-uppercase text-white">site map</span>
            <!-- menus -->
            <div class="d-flex">
              <ul class="footer-right-menu">
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
              </ul>

              <!-- right menu -->
              <ul class="footer-right-menu ms-lg-5">
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
                <li>
                  <a href="#" class="text-white d-flex">Menu</a>
                </li>
              </ul>
            </div>
            <!-- end of menus -->
          </div>
          <!-- end of right footer -->
        </div>

        <!-- powered -->
        <div class="mt-4 d-flex justify-content-center powered">
          <span class="text-white">Powered by</span>
          <a href="#" class="text-white ms-1">GoBuddy</a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Footer",
  components: {},
});
</script>

<style lang="scss">
.footer {
  padding-top: 45px;
  padding-bottom: 45px;
  background-color: #324158;
}

.footer-brand-name {
  font-size: 36px;
}

.footer-social {
  font-size: 40px;
  margin-right: 30px;
}

.footer-right-menu {
  list-style: none;
  margin: 0;
  padding: 0;
  margin-top: 25px;
}

.footer-right-menu > li {
}

.footer-right-menu > li > a {
  text-decoration: none;
  opacity: 0.8;
  margin-bottom: 25px;
}

.powered {
  opacity: 0.8;
}
</style>
