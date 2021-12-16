<template>
  <footer class="main-footer">
    <div class="container d-flex justify-content-center">
      <figure class="main-footer__services up">
        <img src="@/assets/images/chat.png" alt="chatting" />
      </figure>
      <div>
        <figure>
          <img src="@/assets/images/zid-logo-white.png" alt="zid-logo" />
        </figure>
        <div
          class="social-icons d-flex align-items-start justify-content-center"
        >
          <img
            class="social-icon"
            src="@/assets/icons/social/youtube.svg"
            alt="youtube"
          />
          <img
            class="social-icon"
            src="@/assets/icons/social/linkedin.svg"
            alt="linkedin"
          />
          <img
            class="social-icon"
            src="@/assets/icons/social/insta.svg"
            alt="instagram"
          />
          <img
            class="social-icon"
            src="@/assets/icons/social/twitter.svg"
            alt="twitter"
          />
        </div>
      </div>
      <figure class="main-footer__services chatting">
        <img src="@/assets/images/up.png" alt="chatting" />
      </figure>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SiteFooter",
};
</script>

<style lang="scss">
.main-footer {
  background-color: #835d9d;
  padding-top: 1.875rem;
  padding-bottom: 80px;
  text-align: center;
  position: relative;
  .social-icons {
    margin-top: 1.875rem;
    .social-icon {
      margin-right: 1.875rem;
      &:first-of-type {
        margin-right: 0;
      }
    }
  }

  &__services {
    position: absolute;
    bottom: 0;
    &.chatting {
      left: 2%;
    }
    &.up {
      right: 4%;
    }
  }
}
</style>
