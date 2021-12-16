<template>
  <!-- start our uniq-app -->
  <section class="uniq-app">
    <div class="container">
      <header class="text-center uniq-app__main-header">
        <h3>التطبيقات المميزة</h3>
        <p>تطبيقات تقدم حلول وخدمات مميزة نوصي بتجربتها</p>
      </header>
      <div class="row">
        <div class="col-md-3" v-for="item in items" :key="item">
          <div class="uniq-card d-flex">
            <figure class="uniq-card__img">
              <img src="@/assets/images/kumra.png" alt="kumra imgae" />
            </figure>
            <div>
              <header class="uniq-card__header align-items-center">
                <div class="d-flex">
                  <h5>قمرة</h5>
                  <div class="d-flex align-items-center">
                    <img src="@/assets/icons/star.svg" alt="go-ahead" />
                    <span class="uniq-card__number">5</span>
                  </div>
                </div>
                <p class="uniq-card__developer">
                  تطوير:
                  <span class="name">عمر برهوم</span>
                </p>
              </header>
              <p class="uniq-card__content">
                نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك نظام الولاء الأمثل
                الذي يمكنك من رفع مبيعاتك
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="text-center uniq-app__btn">
        <Btn />
      </div>
    </div>
  </section>
  <!-- end our uniq-app -->
</template>

<script>
import Btn from "../Btn";
export default {
  name: "uniq-app",
  components: {
    Btn,
  },
  data: () => ({
    items: 4,
  }),
};
</script>

<style lang="scss">
.uniq-app {
  padding: 11.9375rem 0;
  &__main-header {
    margin-bottom: 40px;
    h3 {
      font-size: 1.5rem;
      font-weight: 400;
      margin-bottom: 0.625rem;
    }
  }
  .uniq-card {
    background: #f7f7f7;
    border-radius: 0.625rem;
    padding: 1.25rem 0.4375rem;
    &__img {
      margin: 0 0 0 10px;
    }

    &__header {
      h5 {
        font-size: 1rem;
        font-weight: 400;
        color: var(--main-purble);
        margin-bottom: 0;
        margin-left: 0.9375rem;
      }
    }

    &__number {
      color: #45a787;
      font-size: 0.875rem;
    }

    p {
      font-size: 0.625rem;
    }
    &__content {
      margin-bottom: 0;
    }
    &__developer {
      line-height: 1.5;
      margin-left: 5px;
      .name {
        color: rgba(0, 0, 0, 0.49);
      }
    }
  }
}

@include to-tablet-sm {
  .uniq-app {
    .uniq-card {
      margin-bottom: 1rem;
    }
  }
}
@include tablet {
  .uniq-app {
    .uniq-card {
      flex-direction: column;
      text-align: center;
      &__img {
        margin-bottom: 1rem;
      }
      &__header {
        & > div {
          justify-content: center;
        }
      }
    }
  }
}
</style>
