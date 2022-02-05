<template>
  <header class="main-header">
    <div class="nav__container">
      <a href="/">
        <img src="@/assets/text.svg" alt="Jurobtics logo" class="mh-logo" />
      </a>
      <nav class="main-nav">
        <ul class="main-nav-list">
          <li>
            <a href="/team">Team</a>
          </li>
          <li>
            <a href="/kontakt">Kontakt</a>
          </li>
          <li>
            <a href="/impressum">Impressum</a>
          </li>
          <li>
            <Button href="#" text="Unterstüzen"></Button>
          </li>
        </ul>
      </nav>
      <!-- <span class="material-icons"> menu </span> -->
    </div>
  </header>
</template>
<script>
import Button from '@/components/Button.vue';

export default {
  name: 'Navbar',
  components: {
    Button,
  },
};
</script>
<style scoped lang="scss">
.nav__container {
  width: 90vw;
  max-width: 100%;
  padding: 20px;
  margin: 0 auto;
  border-radius: 0 0 1rem 1rem;
}

.main-header .nav__container {
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-wrap: wrap;
  background: lightgrey;

  img {
    max-width: 100%;
    height: auto;
    width: 10rem;
  }

  .main-nav {
    ul {
      margin: 1em 0 0.5em;
      text-align: center;

      li {
        display: inline;

        a {
          display: inline-block;
          text-decoration: none;
          color: #000;
          padding: 0.5em 1.5em;
          transition: 0.25s;
        }
        :hover {
          color: #ee7a1b;
        }
      }
    }
  }
}

@media (min-width: 960px) {
  .main-header .nav__container {
    justify-content: space-between;
  }
}

@media screen and (max-width: 761px) {
  .main-header .nav__container {
    flex-direction: column;
  }
}
</style>
