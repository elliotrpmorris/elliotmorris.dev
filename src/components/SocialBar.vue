<template>
<nav class="em-social-bar">
  <a class="em-social-bar__link" href="https://github.com/elliotrpmorris"><img class="em-social-bar__img" src="../assets/svg/github.svg" alt="Github Icon"></a>
  <a class="em-social-bar__link" href="https://www.linkedin.com/in/elliotrpmorris"><img class="em-social-bar__img" src="../assets/svg/linkedin.svg" alt="Linkedin Icon"></a>
  <a class="em-social-bar__link" href="https://twitter.com/elliotrpmorris"><img class="em-social-bar__img" src="../assets/svg/twitter.svg" alt="Twitter Icon"></a>
</nav>
</template>

<script>
export default {
  name: 'socialBar',
};
</script>

<style scoped lang="scss">
@import "../assets/scss/app";

.em-social-bar{

  &__link{
    margin-right: space(16);

    &:last-child{
      margin-right: 0;
    }

    &:hover{
      .em-social-bar__img{
        animation-name: pulse;
        animation-duration: 1s;
        animation-timing-function: linear;
        animation-iteration-count: infinite;
        cursor: pointer !important;
      }

    }
  }

  &__img{
    display: inline-block;
    box-shadow: 0 0 1px rgba(0, 0, 0, 0);
    transform: perspective(1px) translateZ(0) ease-out;
  }
}

@keyframes pulse {
  25%{
    transform: scale(1.1);
  }
  75%{
    transform: scale(0.95);
  }
}
</style>
