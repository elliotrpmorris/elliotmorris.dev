<template>
  <header>
    <em-container>
      <em-nav/>
    </em-container>
  </header>
</template>

<script>
import EmContainer from '@/components/Container.vue';
import EmNav from '@/components/Navigation.vue';

export default {
  name: 'pageHeader',

  components: {
    EmContainer,
    EmNav,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";
</style>
