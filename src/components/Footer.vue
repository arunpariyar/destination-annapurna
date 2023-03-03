<template>
  <div class="section footer">
    <div class="footer__logobox">
      <img
        class="logo"
        src="../assets/images/logo.svg"
        alt="Destination Annapurna Logo"
      />
    </div>
    <div class="footer__about">
      <p>
        Destination Annnapura is an indendent company dedictated to the making
        the Annapurna region accessible to adventurers from all over the world.
        We are commited also to the locals of the Annapurana region to assist in
        the protection the nature and ensure sustainablity.
      </p>
    </div>
    <a href="#" class="btn">Tell me More ! </a>
    <div class="footer__links">
      <ul class="footer__links--navigation">
        <li>About</li>
        <li>Impressium</li>
        <li>Press</li>
        <li>Jobs</li>
      </ul>
      <ul class="footer__links--socialmedia">
        <li><i class="fab fa-instagram"></i></li>
        <li><i class="fab fa-facebook-square"></i></li>
        <li><i class="fab fa-twitter-square"></i></li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style lang="scss">
.logo {
  background-color: rgba(#ffffff, 0.6);
  border-radius: 100px;
  width: 75px;
  height: 75px;
  padding-top: 6px;
}
.footer {
  padding: 5rem 0;
  background-color: var(--earth);
  grid-column: fullbleed-start / fullbleed-end;

  letter-spacing: 1px;
  font-size: 1.4rem;
  font-weight: 300;
  text-align: center;

  color: white;
  &__logobox {
    display: flex;
    justify-content: center;
    margin-bottom: 5rem;
  }
  &__about {
    width: 50%;
    margin: 5rem auto;
  }

  &__links {
    margin: 10rem 5rem 0 5rem;
    display: flex;
    justify-content: space-between;
    &--navigation {
      display: flex;
      list-style: none;
      align-items: center;
      text-transform: uppercase;
      letter-spacing: 1px;

      & > li {
        cursor: pointer;
        margin: 0 2rem;
        transition: all 0.2s;
      }
      & > li:hover {
        color: var(--brown);
        transform: translateY(-3px);
      }
    }

    &--socialmedia {
      display: flex;
      list-style: none;
      text-transform: uppercase;
      align-items: center;
      letter-spacing: 1px;
      & > li {
        font-size: 2.5rem;
        cursor: pointer;
        margin: 0 2rem;
        transition: all 0.2s;
      }
      & > li:hover {
        color: var(--brown);
      }
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
