<template>
  <div class="hero">
    <header class="hero__header text-center">
      <h2 class="purble-text">طور متجرك ووسع افاق تجارتك مع سوق تطبيقات زد</h2>
      <p>
        طور تجارتك من خلال تطبيقات و حلول زد التي تساعدك
        <br />
        في نمو أرباحك عبر إدارة عمليات متجرك بشكل فعال وأحترافي
      </p>
      <Btn />
    </header>
    <section class="hero__show">
      <Fig>
        <img
          class="main-img"
          src="@/assets/images/Intro.png"
          alt="our-applications"
        />
      </Fig>
    </section>
  </div>
</template>

<script>
import Fig from "./Fig";
import Btn from "../Btn";
export default {
  components: {
    Fig,
    Btn,
  },
};
</script>
<style lang="scss">
.hero {
  &__header {
    margin-bottom: 2.5rem;
    h2 {
      font-size: 2.25rem;
      font-weight: 700;
    }
    p {
      margin: 20px 0 40px 0;
      font-size: 18px;
      font-weight: 400;
      padding: 16px 48px;
    }
  }
  &__show {
    display: flex;
    justify-content: center;
    margin-top: 5rem;
    margin-bottom: 12.5rem;
  }
}
</style>
