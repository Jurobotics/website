<template>
  <header>
    <a href="#">
      <img class="text" src="@/assets/text.svg" alt="Logo with text Jurobotics" />
    </a>
    <Button href="impressum" text="Impressum"></Button>
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
