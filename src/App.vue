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
@use "./styles/generals.scss" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/partials/variables" as *;
</style>
