<template>
  <div class="nav">
    <div class="nav_logo">
      <img class="logo" src="../assets/images/logo.svg" alt="Mountains" />
    </div>
    <ul class="nav__links">
      <li class="nav__item">
        <a class="nav__link" href="#section--1">Adventures</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#section--2">Impressions</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#">Make it happen</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Navigation",
};
</script>
<style lang="scss" scoped>
@import "../assets/mixins.scss";
.nav {
  display: flex;
  justify-content: space-between;
  padding: 4rem 8rem;
  align-items: center;
  @include respond(tab-land) {
    padding: 4rem 4rem;
  }
  @include respond(tab-port) {
    padding: 4rem 2rem;
  }

  &__links {
    display: flex;
    align-items: center;
    justify-content: space-between;
    list-style: none;
    @include respond(tab-port) {
      display: block;
    }
  }
  &__link:link,
  &__link:visited {
    letter-spacing: 1.5px;
    text-decoration: none;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: white;
    margin: 0 3rem;
    transition: all 0.2s;
    padding-bottom: 1.5rem;
    border-bottom: 2px solid transparent;
  }
  &__link:hover {
    padding-bottom: 1.5rem;
    border-bottom: 2px solid var(--brown);
  }
  &__link:active {
    padding-bottom: 1.5rem;
    border-bottom: 2px solid transparent;
  }
}

.logo {
  background-color: rgba(#ffffff, 0.6);
  border-radius: 100px;
  width: 75px;
  height: 75px;
  padding-top: 6px;
}

.logo-sticky {
  width: 55px;
  height: 55px;
  padding-top: 6px;
}

.sticky {
  position: fixed;
  background-color: rgba(#5f4620, 0.95);
  position: fixed;
  top: 0;
  right: 0;
  width: 100vw;
  z-index: 9999;
  padding: 1.5rem 8rem;
}
</style>
