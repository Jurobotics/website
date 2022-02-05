<template>
  <a class="button" :href="href">{{ text }}</a>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    href: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.button {
  text-decoration: none;
  color: #000;
  font-size: 1.2rem;
  padding: 12px 17px;
  border-radius: 10px;
  background: #ee7a1a8c;
  transition: 0.5s;
}
:hover {
  background: #ee7a1a;
  transition: 0.5s;
}
</style>
