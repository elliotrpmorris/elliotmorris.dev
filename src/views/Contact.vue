<template>
  <em-container>
    <em-row>
      <em-column eight>
        <em-card alto>
          <em-heading xlarge mineShaft>Contact me!</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
            <a
              class="link"
              href="mailto:hello@elliotmorris.dev"
            >hello@elliotmorris.dev</a>
          </em-page-text>
          <img class="contact__img" src="../assets/me.jpg" alt="Image of Elliot Morris">
          <em-social-bar/>
        </em-card>
      </em-column>
    </em-row>
  </em-container>
</template>

<script>
import EmContainer from '@/components/Container.vue';
import EmRow from '@/components/Row.vue';
import EmColumn from '@/components/Column.vue';
import EmPageText from '@/components/PageText.vue';
import EmHeading from '@/components/Heading.vue';
import EmCard from '@/components/Card.vue';
import EmSocialBar from '@/components/SocialBar.vue';

export default {
  name: 'contact',
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmPageText,
    EmHeading,
    EmCard,
    EmSocialBar,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.contact {
  &__img {
    border-radius: 50%;
    width: 150px;
    margin: 0 auto space(24) auto;
  }
}
</style>
