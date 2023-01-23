<template lang="">
  <div class="container-fluid">
    <!-- row 1 -->
    <div class="row d-flex text-white">
      <!-- address section -->
      <section class="col-4">
        <h4>Address</h4>
        <p v-for="(item, index) in addressSect">{{ addressSect[index] }}</p>
      </section>

      <!-- explore section -->
      <section class="col-2">
        <h4>Explore</h4>
        <ul v-for="(item, index) in exploreSect" class="list-unstyled">
          <li>
            <a href="/" class="text-decoration-none">{{
              exploreSect[index]
            }}</a>
          </li>
        </ul>
      </section>

      <!-- information section -->
      <section class="col-2">
        <h4>Information</h4>
        <ul v-for="(item, index) in informationSect" class="list-unstyled">
          <li>
            <a href="/" class="text-decoration-none">{{
              informationSect[index]
            }}</a>
          </li>
        </ul>
      </section>

      <!-- instagram section -->
      <section class="col-4">
        <h4>Instagram</h4>
      </section>
    </div>

    <!-- row 2 -->
    <div class="row rights">
      <div class="col-12 d-flex justify-content-center text-white">
        &copy; 2020 Maxcoach. All Rights Reserved
      </div>
    </div>
  </div>
</template>

<!-- script -->
<script>
export default {
  data() {
    return {
      addressSect: [
        "382 NE 191st St # 87394 Miami, FL 33179-3899",
        "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)",
        "support@maxcoach.com",
      ],
      exploreSect: [
        "Start here",
        "Success story",
        "Blog",
        "Courses",
        "Contact us",
      ],
      informationSect: [
        "Membership",
        "Purchase Guide",
        "Privacy policy",
        "Terms of services",
      ],
    };
  },
};
</script>

<!-- style -->
<style lang="scss" scoped>
@use "../styles/generals.scss";
@use "../styles/partials/mixins";
@use "../styles/partials/variables";

.rights {
  padding-top: 100px;
}
</style>
