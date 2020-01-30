<template>
  <div class="grid-row">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'Row',
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.grid-row {
  display: -ms-flexbox;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  margin-left: ceil($base-spacing / -2);
  margin-right: floor($base-spacing / -2);

  &--no-wrap {
    flex-wrap: nowrap;
  }
}
</style>
