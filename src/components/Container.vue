<template>
  <div class="grid-container" :class="classes">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'container',

  props: {
    fluid: {
      type: Boolean,
      required: false,
      default: false,
    },
  },

  computed: {
    classes() {
      return {
        'grid-container--fluid': this.fluid,
      };
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.grid-container {
  max-width: $xl-screen-width;
  margin: 0 auto;

  @include bp-md {
    padding: 0 $base-spacing;
  }

  &--fluid {
    margin: 0;
    max-width: 100%;
  }
}
</style>
