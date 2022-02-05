<template>
  <Navbar></Navbar>
  <router-view />
</template>
<script>
import Navbar from '@/components/Navbar.vue';

export default {
  components: {
    Navbar,
  },
};
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Open Sans', sans-serif;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Poppins', sans-serif;
}

body {
  background: rgba(53, 53, 53, 0.1);
}

@media screen and (max-width: 731px) {
  .logo a img:hover {
    transform: scale(1.2) rotate(5deg) !important;
  }
}

.container {
  width: 100%;
  padding: 17px;
  box-shadow: 8px 8px 15px 7px rgb(0 0 0 / 10%);
  border-radius: 10px;
  max-width: 90%;
  margin: auto;
  margin-top: 2.5rem;
  margin-bottom: 5rem;
  background: #fff;
}

.logo {
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 80vh;
  width: 100%;
}

.logo a img {
  width: 100%;
  transition: 0.2s;
}

.logo a img:hover {
  transform: scale(1.5) rotate(5deg);
  transition: 0.2s;
}
</style>
