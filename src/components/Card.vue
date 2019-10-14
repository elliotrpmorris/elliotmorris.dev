<template>
  <article class="em-card" :class="classes">
    <slot/>
  </article>
</template>

<script>

export default {
  name: 'card',

  props: {
    alto: {
      type: Boolean,
      required: false,
      default: false,
    },
    white: {
      type: Boolean,
      required: false,
      default: false,
    },
  },

  computed: {
    classes() {
      return {
        'em-card--alto': this.alto,
        'em-card--white': this.white,
      };
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-card {
  display: flex;
  flex-direction: column;
  z-index: 1;
  position: relative;
  padding: space(40);

  @include bp-md {
    padding: space(80);
  }

  &:hover {
    &::before {
      box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25),
        0 10px 10px rgba(0, 0, 0, 0.22);
      transform: rotate(2deg) scale(1.01);
    }
  }

  &::before {
    content: " ";
    display: block;
    height: 100%;
    left: 0;
    position: absolute;
    top: 0;
    width: 100%;
    z-index: -1;
    transform: rotate(-2deg);
    box-shadow: -1px 1px 24px 0 rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease-in-out;
  }

  &--alto {
    background-color: $alto;
    color: $mine-shaft;

    &::before {
      background-color: $alto;
    }
  }

  &--white {
    background-color: $white;
    color: $mine-shaft;

    &::before {
      background-color: $white;
    }
  }
}
</style>
