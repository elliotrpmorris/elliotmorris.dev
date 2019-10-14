<template>
  <main id="app">
    <em-page-header/>
    <router-view/>
  </main>
</template>

<script>
import EmPageHeader from '@/components/PageHeader.vue';

export default {
  components: {
    EmPageHeader,
  },
};
</script>

<style lang="scss">
@import "../src/assets/scss/app";
</style>
