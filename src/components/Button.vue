<template>
  <button href="#section--1" class="btn-submit btnToTrips">
    Explore Adventures
  </button>
</template>
<script></script>
<style lang="scss" scoped>
.btn:link,
.btn:visited {
  background-color: var(--brown);
  text-transform: uppercase;
  border-radius: 30px;
  font-weight: 300;
  padding: 1.5rem 3rem;
  text-decoration: none;
  color: white;
  letter-spacing: 1px;
  transition: all 0.2s;
  display: inline-block;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 1.5rem 1rem rgba(255, 255, 255, 0.15);
}
.btn:active {
  transform: translateY(-1px);
  box-shadow: 0 1.5rem 1rem rgba(0, 0, 0, 0.15);
  color: var(--earth);
}

.btn-trip {
  padding: 0.5rem 1.5rem !important;
}

.btn-trip:hover {
  box-shadow: 0 1.5rem 1rem rgba(0, 0, 0, 0.15) !important;
}

.btn-trip:active {
  color: white;
}

.btn-submit {
  margin-top: 4rem;
  background-color: var(--brown);
  text-transform: uppercase;
  border-radius: 30px;
  font-weight: 500;
  padding: 1.5rem 2rem;
  text-decoration: none;
  color: white;
  letter-spacing: 1px;
  transition: all 0.2s;
  border: none;
  cursor: pointer;
  &:focus {
    outline: none;
  }
}

.btn-submit:hover {
  transform: translateY(-3px);
  box-shadow: 0 1.5rem 1rem rgba(255, 255, 255, 0.15);
}
.btn-submit:active {
  transform: translateY(-1px);
  box-shadow: 0 1.5rem 1rem rgba(0, 0, 0, 0.15);
}
</style>
