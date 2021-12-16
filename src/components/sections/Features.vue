<template>
  <!-- start features -->
  <section class="features">
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="features__content">
            <header>
              <h3>كل ما تحتاجه لنمو متجرك في مكان واحد</h3>
              <p>
                مميزات سوق تطبيقات زد تساعدك في سهولة و سرعة الاستفادة من خدمات
                وحلول سوق التطبيقات لنمو متجرك و مضاعفة أرباحك
              </p>
            </header>
            <ul class="features__items">
              <li class="d-flex align-items-end">
                <div class="icon">
                  <img
                    src="@/assets/icons/features/mail.svg"
                    alt="easy-to-control"
                  />
                </div>
                <p>سهولة أدارة وتفعيل تطبيقاتك من نفس لوحة تحكم متجرك</p>
              </li>
              <li class="d-flex align-items-end">
                <div class="icon">
                  <img src="@/assets/icons/features/chat.svg" alt="support" />
                </div>
                <p>دعم فني وتقني متكامل متوفر علي مدار الساعة</p>
              </li>
              <li class="d-flex align-items-end">
                <div class="icon">
                  <img
                    src="@/assets/icons/features/hand.svg"
                    alt="free-trial"
                  />
                </div>
                <p>أسعار تنافسية مع تجربة مجانية و باقات أشتراك متنوعة</p>
              </li>
            </ul>
            <Btn />
          </div>
        </div>
        <div class="col-lg-6">
          <Fig>
            <img
              class="main-img"
              src="@/assets/images/zidapp.png"
              alt="our-applications"
            />
          </Fig>
        </div>
      </div>
    </div>
  </section>
  <!-- end features -->
</template>

<script>
import Fig from "./Fig";
import Btn from "../Btn.vue";
export default {
  name: "Features",
  components: {
    Fig,
    Btn,
  },
};
</script>

<style lang="scss">
.features {
  padding: 57px 0;
  background: #fafafc;

  &__content header {
    h3 {
      font-size: 24px;
      color: var(--main-purble);
      font-weight: 700;
      margin-bottom: 20px;
    }
    p {
      font-size: 16px;
      margin-bottom: 20px;
    }
  }

  &__items {
    margin-bottom: 2.5rem;
    li {
      font-size: 14px;
      margin-bottom: 20px !important;
    }
  }
  .icon {
    width: 3.125rem;
    height: 3.125rem;
    box-shadow: 0.1875rem 0.125rem 0.5625rem 0 #bfbfbf;
    margin-left: 1.25rem;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;

    img {
      width: 50%;
      height: 50%;
    }
  }
  .fig {
    align-items: end;
    height: 100%;
    img {
      &.main-img {
        width: 115%;
      }
      &.ellipse {
        right: -15%;
        top: 30%;
      }
      &.dot-pattern {
        left: -10%;
        top: 0;
      }
    }
  }
}

@include to-tablet-lg {
  .features {
    &__content {
      text-align: center;
    }
    &__items {
      margin-bottom: 0 !important;
      li {
        flex-direction: column;
        align-items: center !important;
      }
      .icon {
        margin-bottom: 1rem;
      }
    }
    .btn.main-btn {
      margin-bottom: 2.5rem;
    }
  }
}
</style>
