<template>
  <header class="main-header menu-absolute">
    <!--Header-Upper-->
    <div class="header-upper">
      <div class="container clearfix">
        <div class="header-inner rpy-10 rel d-flex align-items-center">
          <div class="logo-outer">
            <div class="logo">
              <NuxtLink href="/"
                ><img
                  src="/assets/images/logos/beyaz-logo.png"
                  alt="Logo"
                  title="Logo"
                  width="180"
              /></NuxtLink>
            </div>
          </div>

          <div class="nav-outer ms-lg-auto clearfix">
            <!-- Main Menu -->
            <nav class="main-menu navbar-expand-lg">
              <div class="navbar-header py-10">
                <div class="mobile-logo">
                  <NuxtLink href="/">
                    <img
                      src="/assets/images/logos/beyaz-logo.png"
                      alt="Logo"
                      title="Logo"
                      width="180"
                    />
                  </NuxtLink>
                </div>

                <!-- Toggle Button -->
                <button
                  type="button"
                  class="navbar-toggle"
                  data-bs-toggle="collapse"
                  data-bs-target=".navbar-collapse"
                >
                  <span class="icon-bar"></span>
                  <span class="icon-bar"></span>
                  <span class="icon-bar"></span>
                </button>
              </div>

              <div class="navbar-collapse collapse clearfix">
                <ul
                  class="navigation onepage clearfix"
                  v-if="singlePage == true"
                >
                  <li><a href="/about">kurumsal</a></li>
                  <li><a href="/services">hizmetlerimiz</a></li>
                  <li><a href="/projects">referanslar</a></li>
                  <li><a href="/blog">blog</a></li>
                  <li><a href="/contact">iletişim</a></li>
                </ul>
                <HeadersNav v-else />
              </div>
            </nav>
            <!-- Main Menu End-->
          </div>

          <!-- Nav Search -->
          <!-- <HeadersSearch /> -->

          <!-- Menu Button -->
          <div class="menu-btns ms-lg-auto">
            <NuxtLink @click="toggleSidebar()" class="theme-btn style-two me-4"
              >Proje Başlat <i class="far fa-arrow-left"></i
            ></NuxtLink>
            <!-- menu sidbar -->
            <div class="menu-sidebar">
              <button class="bg-transparent" @click="toggleSidebar()">
                <img
                  src="/assets/images/icons/toggler-white.svg"
                  alt="Toggler"
                />
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!--End Header Upper-->
  </header>
  <HeadersSidebar />
</template>

<script>
export default {
  name: "Header2",
  props: {
    singlePage: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
    toggleSidebar() {
      document.querySelector("body").classList.add("side-content-visible");
    },
  },
};
</script>
