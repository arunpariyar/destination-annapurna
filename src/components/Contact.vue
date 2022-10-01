<script>
export default {
  name: "Contact",
};
</script>
<template>
  <div class="section-heading" id="section--3">Your Adventure Begins</div>
  <section class="section booking">
    <div class="booking__container">
      <form action="" class="form">
        <h2 class="form__heading">Make it happen</h2>
        <div class="form__group">
          <input
            type="text"
            class="form__input"
            placeholder="Full Name"
            id="name"
            required
          />
          <label for="name" class="form__label"></label>
        </div>
        <div class="from__group">
          <input
            type="email"
            class="form__input"
            placeholder="Email Address"
            id="email"
            required
          />
          <label for="email" class="form__label"></label>
        </div>
        <div class="from__group">
          <button class="btn-submit">sign me up !</button>
        </div>
      </form>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "../assets/mixins";
.section-heading {
  font-family: var(--font-heading);
  text-transform: uppercase;
  text-align: center;
  font-size: 3.5rem;
  color: var(--earth);
  letter-spacing: 15px;
  margin: 8rem 0;
}

.form {
  width: 50%;
  padding: 5rem;
  @include respond(tab-port) {
    width: 100%;
  }

  &__group:not(:last-child) {
    margin-bottom: 3rem;
  }

  &__heading {
    font-family: var(--font-heading);
    font-size: 4rem;
    text-transform: uppercase;
    color: var(--earth);
    letter-spacing: 2px;
    margin-bottom: 2rem;
  }

  &__input {
    padding: 1.5rem 2rem;
    border-radius: 2px;
    background-color: rgba(white, 0.5);
    border: none;

    border-bottom: 3px solid transparent;
    width: 100%;
    display: block;

    &:focus {
      outline: none;
      box-shadow: 0 1rem 2rem rgba(black, 0.2);
      border-bottom: 3.5px solid var(--brown);
    }
  }
}

.booking {
  padding: 10rem 0;
  background-color: var(--brown);

  &__container {
    margin: auto 15rem;
    background-image: linear-gradient(
        90deg,
        rgba(#fff, 0.7) 0%,
        rgba(#fff, 0.7) 50%,
        transparent 50%
      ),
      url(../assets/images/booking.jpg);

    background-size: cover;
    background-position: center;
    border-radius: 3px;
    box-shadow: 0 1.5rem 4rem rgba(black, 0.5);

    @include respond(tab-port) {
      background-image: linear-gradient(
          90deg,
          rgba(#fff, 0.7) 0%,
          rgba(#fff, 0.7) 50%,
          rgba(#fff, 0.7) 100%
        ),
        url(../assets/images/booking.jpg);
    }
  }
}
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
