<template lang="">
  <!-- event of the year -->
  <div class="container d-flex justify-content-center gap-4 m-3">
    <span>Starts TOMORROW! Our biggest event of the year...</span>
    <div></div>
    <button class="btn">Get ticket</button>
  </div>

  <!-- proper header -->
  <div class="container" style="height: 75px">
    <div class="row d-flex align-items-center">
      <!-- logo -->
      <div class="col-4">
        <div class="pLogo">
          <a href="/"
            ><img src="src/assets/images/dark-logo.png" alt="logo"
          /></a>
        </div>
      </div>

      <!-- nav -->
      <div class="col-4 d-flex justify-content-center">
        <navbar />
      </div>

      <!-- socials -->
      <div class="col-4 d-flex justify-content-end">
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

.pLogo {
  width: 150px;
  img {
    width: 100%;
  }
}
</style>
