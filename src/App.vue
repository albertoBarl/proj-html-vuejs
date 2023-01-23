<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

components: {
  Header;
  Footer;
}
</script>

<template>
  <Header />
  <Footer />
</template>

<style lang="scss" scoped>
@use "./styles/generals.scss";
@use "./styles/partials/mixins";
@use "./styles/partials/variables";
</style>
