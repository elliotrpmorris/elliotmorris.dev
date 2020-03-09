<template>
  <em-container>
    <em-row>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Asda Money</em-heading>
          <em-page-text>
            In my last role i was the main developer for the ASDA money site.
            Doing frontend work using technologies like AngularJS & Jquery
            and backend work with Umbraco.
            <hr>
            <a class="link" href="https://money.asda.com">View Site!</a>
          </em-page-text>
          <details class="em-accordion">
            <summary>Key features I built:</summary>
            <figure class="em-accordion__content">
              <li>Current home page</li>
              <li>Product page hero</li>
              <li>Custom plugin for the Umbraco admin</li>
            </figure>
          </details>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Leeds Rhinos</em-heading>
          <em-page-text>
            On this project i was tasked with creating all of the frontend templates
            which consisted of HTML, JS and CSS. I also worked on the Wordpress plugin
            which allowed us to get data from a feed provided by OPTA
            which enabled us to serve stats on the site.
            <hr>
            <a class="link" href="https://www.therhinos.co.uk/">View Site!</a>
          </em-page-text>
          <details class="em-accordion">
            <summary>Key features I built:</summary>
            <figure class="em-accordion__content">
              <li>Responsible for the frontend template code</li>
              <li>SQL Queries for getting data from OPTA feed</li>
              <li>PHP code for the Wordpress OPTA plugin</li>
            </figure>
          </details>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Clandestine Labs</em-heading>
          <em-page-text>
            This site is built in react, it acts as information site for
            freelance projects i work on such as website development &
            website hosting.
            <hr>
            <a class="link" href="https://labs.clandestine.tech">View Site!</a>
          </em-page-text>
        </em-card>
      </em-column>
      <em-column six>
        <em-card alto>
          <em-heading large mineShaft>Want to see your project here?</em-heading>
          <em-page-text>
            Need help with a cool project?
            Email me!
          </em-page-text>
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
  name: 'work',
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

.em-accordion {
  font-family: $font-primary;
  font-size: $font-size-body-m;
  color: $dove-grey;

  &__content {
    font-size: $font-size-base;
    text-align: left;
    padding-top: space(16);
  }
}
</style>
