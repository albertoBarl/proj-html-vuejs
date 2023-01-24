<template lang="">
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
        <div class="navigation d-flex gap-5">
          <ul
            v-for="(item, index) in navbar"
            :key="index"
            class="list-unstyled"
          >
            <li class="d-flex">
              {{ navbar[index].section }} <span class="ms-2">&darr;</span>
            </li>
          </ul>
        </div>
      </div>

      <!-- socials -->
      <div class="col-4 d-flex justify-content-end">
        <socials />
      </div>
    </div>
  </div>
</template>

<!-- script -->
<script>
import socials from "./elements/socials.vue";

export default {
  components: {
    socials,
  },
  props: {
    navbar: Array,
  },
};
</script>

<!-- style -->
<style lang="scss" scoped>
@use "../styles/generals.scss" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;

.pLogo {
  width: 150px;
  img {
    width: 100%;
  }
}
</style>
