<template>
  <p class="text" :class="classes">
    <slot/>
  </p>
</template>

<script>
export default {
  name: 'pageText',

  props: {
    white: {
      type: Boolean,
      required: false,
      default: false,
    },
    mineShaft: {
      type: Boolean,
      required: false,
      default: false,
    },
    alto: {
      type: Boolean,
      required: false,
      default: false,
    },
  },

  computed: {
    classes() {
      return {
        'text--white': this.white,
        'text--mineshaft': this.mineShaft,
        'text--alto': this.alto,
      };
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.text {
  font-size: $base-font-size;
  font-family: $font-primary;

  &--white {
    color: $white;
  }

  &--mineshaft {
    color: $mine-shaft;
  }

  &--alto {
    color: $alto;
  }
}
</style>
