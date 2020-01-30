<template>
  <em-container>
    <em-row>
      <em-column class="about__content" twelve>
        <em-card alto>
          <em-heading mineShaft xlarge>About me</em-heading>
          <em-page-text mineShaft>
            I am a full stack developer from the UK,
            currently working for Next in South Elmsall near Pontefract.
            Working on creating web apps for internal warehouse systems using
            .Net Core, EF Core and Angular.
          </em-page-text>
          <em-page-text mineShaft>
            As an advocate for all things web it is important to me
            that the product is usable by all, ensuring
            I am following high accessibility standards
            as well as achieving the best performance and producing
            top quality code.
          </em-page-text>
          <em-heading mineShaft>Heres some tech that i like to use:</em-heading>
          <ul>
            <li>HTML5, CSS3, JS (ES6), Node</li>
            <li>Angular, Angular.js</li>
            <li>Vue.js</li>
            <li>React</li>
            <li>.Net (C#), .Net Core, EF, Umbraco</li>
            <li>Php, Laravel, Wordpress, Statamic</li>
            <li>AWS, Azure, Git, Trello</li>
          </ul>
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

export default {
  name: 'about',
  components: {
    EmContainer,
    EmRow,
    EmColumn,
    EmPageText,
    EmHeading,
    EmCard,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.about {
  &__content {
    color: $white;
    font-family: $font-primary;
  }
}
</style>
