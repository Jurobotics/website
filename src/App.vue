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
  font-family: sans-serif;
}

@media screen and (max-width: 731px) {
  .logo a img:hover {
    transform: scale(1.2) rotate(5deg) !important;
  }
}

.container {
  width: 90%;
  padding: 17px;
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

header {
  display: flex;
  padding: 17px;
  background: lightgrey;
  border-radius: 0 0 1rem 1rem;

  justify-content: space-between;
  align-items: center;
}

.text {
  width: 10rem;
}
</style>
