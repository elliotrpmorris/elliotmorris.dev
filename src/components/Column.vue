<template>
  <div class="grid-col" :class="classes">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'column',
  props: {
    one: {
      type: Boolean,
      required: false,
      default: false,
    },
    two: {
      type: Boolean,
      required: false,
      default: false,
    },
    three: {
      type: Boolean,
      required: false,
      default: false,
    },
    four: {
      type: Boolean,
      required: false,
      default: false,
    },
    five: {
      type: Boolean,
      required: false,
      default: false,
    },
    six: {
      type: Boolean,
      required: false,
      default: false,
    },
    seven: {
      type: Boolean,
      required: false,
      default: false,
    },
    eight: {
      type: Boolean,
      required: false,
      default: false,
    },
    nine: {
      type: Boolean,
      required: false,
      default: false,
    },
    ten: {
      type: Boolean,
      required: false,
      default: false,
    },
    eleven: {
      type: Boolean,
      required: false,
      default: false,
    },
    twelve: {
      type: Boolean,
      required: false,
      default: false,
    },
    tOne: {
      type: Boolean,
      required: false,
      default: false,
    },
    tTwo: {
      type: Boolean,
      required: false,
      default: false,
    },
    tThree: {
      type: Boolean,
      required: false,
      default: false,
    },
    tFour: {
      type: Boolean,
      required: false,
      default: false,
    },
    tFive: {
      type: Boolean,
      required: false,
      default: false,
    },
    tSix: {
      type: Boolean,
      required: false,
      default: false,
    },
    tSeven: {
      type: Boolean,
      required: false,
      default: false,
    },
    tEight: {
      type: Boolean,
      required: false,
      default: false,
    },
    tNine: {
      type: Boolean,
      required: false,
      default: false,
    },
    tTen: {
      type: Boolean,
      required: false,
      default: false,
    },
    tEleven: {
      type: Boolean,
      required: false,
      default: false,
    },
    tTwelve: {
      type: Boolean,
      required: false,
      default: false,
    },
    noGutters: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
  computed: {
    classes() {
      return {
        'grid-col--1': this.one,
        'grid-col--2': this.two,
        'grid-col--3': this.three,
        'grid-col--4': this.four,
        'grid-col--5': this.five,
        'grid-col--6': this.six,
        'grid-col--7': this.seven,
        'grid-col--8': this.eight,
        'grid-col--9': this.nine,
        'grid-col--10': this.ten,
        'grid-col--11': this.eleven,
        'grid-col--12': this.twelve,
        'grid-col--t--1': this.tOne,
        'grid-col--t--2': this.tTwo,
        'grid-col--t--3': this.tThree,
        'grid-col--t--4': this.tFour,
        'grid-col--t--5': this.tFive,
        'grid-col--t--6': this.tSix,
        'grid-col--t--7': this.tSeven,
        'grid-col--t--8': this.tEight,
        'grid-col--t--9': this.tNine,
        'grid-col--t--10': this.tTen,
        'grid-col--t--11': this.tEleven,
        'grid-col--t--12': this.tTwelve,
        '-no-gutters': this.noGutters,
      };
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.grid-col {
  box-sizing: border-box;
  text-align: center;
  width: 100%;
  padding: $base-spacing;

  @include bp-md {
    // Column % Tablet
    &--t {
      @for $i from 1 to $total-columns + 1 {
        &--#{$i} {
          width: percentage($i/$total-columns);
        }
      }
    }
  }

  @include bp-lg {
    // Column % Desktop
    @for $i from 1 to $total-columns + 1 {
      &--#{$i} {
        width: percentage($i/$total-columns);
      }
    }
  }
}

.-no-gutters{
  padding: 0;
  margin: 0;
}
</style>
