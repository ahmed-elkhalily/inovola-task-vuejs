<template>
  <button class="btn main-btn">
    <div>
      تصفح التطبيقات
      <img src="@/assets/icons/chevron.svg" alt="goto" />
    </div>
  </button>
</template>

<script>
export default {
  name: "Btn",
};
</script>

<style lang="scss">
/* main-btn */
.btn {
  &.main-btn {
    font-size: 18px;
    border-radius: 0.5625rem;
    font-weight: 600;
    padding: 12px 65.23px;
    color: var(--main-yellow);
    background: var(--main-purble);
  }
  &:hover {
    color: var(--main-yellow) !important;
  }
  img {
    margin-right: 11px;
  }
}

.uniq-app__btn {
  .btn.main-btn {
    margin-top: 2.5rem;
    background: transparent;
  }
}
</style>
