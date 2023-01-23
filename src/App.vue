<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

components: {
  Header;
  Footer;
}
</script>

<template>
  <div class="header">
    <Header />
  </div>
  <div class="footer">
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
@use "./styles/generals.scss" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/partials/variables" as *;

.footer {
  background-color: $d-wall;
  padding: 75px 0px;
}
</style>
