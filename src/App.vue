<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import eventscount from "./components/elements/eventscount.vue";

export default {
  components: {
    Header,
    Footer,
    eventscount,
  },
};
</script>

<template>
  <eventscount />
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

.header {
  background-color: $wall;
  position: fixed;
  width: 100%;
}

.footer {
  background-color: $d-wall;
  padding: 75px 0px;
}
</style>
