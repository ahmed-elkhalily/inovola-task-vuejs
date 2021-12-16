<template>
  <figure class="fig d-flex justify-content-center container">
    <slot class="main-img"></slot>
    <img
      class="dot-pattern"
      src="@/assets/images/Dot-Pattern.png"
      alt="applications-pattern"
    />
    <img
      class="ellipse"
      src="@/assets/images/yellow-ellipse.png"
      alt="applications-pattern"
    />
  </figure>
</template>

<script>
export default {
  name: "Fig",
};
</script>

<style lang="scss">
.fig {
  position: relative;
  img {
    &.main-img {
      position: static;
      z-index: 2;
      width: 90%;
    }
    &.dot-pattern {
      position: absolute;
      left: 0%;
      top: -10%;
      z-index: 1;
    }
    &.ellipse {
      position: absolute;
      right: 1%;
      bottom: -20%;
      z-index: 1;
    }
  }
}
// /*start Hero medias */
@include to-tablet-sm {
  .fig img {
    &.ellipse {
      bottom: -20%;
      width: 250px;
      right: -10%;
    }
  }
}
@include mobile-xs {
  .fig {
    img {
      &.main-img {
        width: 100%;
      }
      &.dot-pattern {
        width: 100px;
        left: -2%;
        top: -20%;
      }
      &.ellipse {
        width: 170px;
        right: -10%;
        bottom: -25%;
      }
    }
  }
}

// @include mobile-sm {
//   .fig img {
//     &.ellipse {
//       width: 280px;
//     }
//   }
// }
</style>
