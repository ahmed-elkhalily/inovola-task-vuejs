<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="@/assets/images/zid-logo.png" alt="zid-logo" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        @click="toggleShow()"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse"
        :class="{ show: show }"
        id="navbarSupportedContent"
      >
        <ul class="navbar-nav mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">الرئيسية</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">التصنيفات</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">التطبيقات</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">طور التطبيق</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data: () => ({
    show: false,
  }),
  methods: {
    toggleShow() {
      this.show = !this.show;
      console.log(this.show);
    },
  },
};
</script>

<style lang="scss">
.navbar {
  margin-bottom: 3.75rem;
  li.nav-item {
    margin-right: 6.25rem !important;
  }

  &.navbar-light .navbar-nav .nav-link {
    color: #000 !important;
    &:hover,
    &:focus {
      color: #000 !important;
    }
  }

  .navbar-collapse {
    height: 0;
    transition: height 0.5s;
  }
  .navbar-collapse.show {
    height: 100%;
    li.nav-item {
      text-align: center;
    }
  }
}
</style>
