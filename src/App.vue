<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
import eventscount from "./components/elements/eventscount.vue";

export default {
  components: {
    // main components
    Header,
    Footer,
    Main,
    // others
    eventscount,
  },
};
</script>

<template>
  <div class="eventscount">
    <eventscount />
  </div>
  <div class="header">
    <Header />
  </div>
  <div class="main">
    <Main />
  </div>
  <div class="footer">
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
@use "./styles/generals.scss" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/partials/variables" as *;

// .eventscount {
// }
.header {
  background-color: $wall;
  // position: fixed;
  // width: 100%;
  // top: 0;
}

.footer {
  background-color: $d-wall;
}
</style>
