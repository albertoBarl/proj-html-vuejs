<template lang="">
  <!-- event of the year -->
  <div class="container d-flex justify-content-center gap-4 m-3">
    <span class="text-white"
      >Starts TOMORROW! Our biggest event of the year...</span
    >
    <div></div>
    <button class="btn">Get ticket</button>
  </div>

  <!-- proper header -->
  <div class="container-fluid">
    <div class="row">
      <!-- logo -->
      <div class="col-4"></div>

      <!-- nav -->
      <navbar class="col-4" />

      <!-- socials -->
      <div class="col-4">
        <socials />
      </div>
    </div>
  </div>
</template>
<script>
import navbar from "./elements/navbar.vue";
import socials from "./elements/socials.vue";

export default {
  components: {
    navbar,
    socials,
  },
};
</script>
<style lang="scss" scoped>
@use "../styles/generals.scss" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;

.btn {
  padding: 3px 40px;
  background-color: $aranciata;
  color: $wall;
  &:hover {
    background-color: $cielo;
    color: $wall;
  }
}
</style>
