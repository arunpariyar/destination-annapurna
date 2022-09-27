<script>
import Navigation from "./Navigation.vue";
import Button from "./Button.vue";
export default {
  name: "Header",
  components: {
    Navigation,
    Button,
  },
};
</script>

<template>
  <section class="header">
    <!-- <a class ="nav__hamburger" href="#"><i class="fas fa-bars"></i></a> -->
    <Navigation />
    <div class="header__text">
      <h2 class="header__text--intro">Experience the best adventures in the</h2>
      <h1 class="header__text--hero">Annapurna<br />himalayas</h1>
      <Button />
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "../assets/mixins.scss";
.header {
  background-image: linear-gradient(rgba(255, 255, 255, 0), rgba(0, 0, 0, 0.6)),
    url(../assets/images/hero.jpg);
  background-size: cover;
  background-position: center;
  height: 96vh;

  position: relative;

  &__text {
    position: absolute;
    top: 70%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    line-height: 1.5;
    &--intro {
      color: white;
      font-size: 2rem;
      letter-spacing: 5px;
      text-transform: uppercase;
      font-family: var(--font-heading);
      @include respond(tab-port) {
        font-size: 1.8rem;
      }
    }
    &--hero {
      margin-bottom: 2rem;
      color: white;
      text-transform: uppercase;
      font-size: 5rem;
      letter-spacing: 21px;
      font-family: var(--font-hero);
      @include respond(tab-port) {
        font-size: 4.5rem;
      }
    }
  }
}
</style>
