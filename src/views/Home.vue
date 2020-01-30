<template>
  <div class="em-home">
    <em-hero/>
    <em-container>
      <em-social-bar class="em-home__social-bar"/>
    </em-container>
  </div>
</template>

<script>
import EmContainer from '@/components/Container.vue';
import EmHero from '@/components/Hero.vue';
import EmSocialBar from '@/components/SocialBar.vue';

export default {
  name: 'home',
  components: {
    EmContainer,
    EmHero,
    EmSocialBar,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-home__social-bar {
  margin: space(32) auto;
  text-align: center;
}
</style>
