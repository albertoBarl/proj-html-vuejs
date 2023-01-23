<template lang="">
  <div class="container-fluid">
    <!-- row 1 -->
    <div class="row d-flex text-white">
      <!-- address section -->
      <section class="col-4">
        <h4>Address</h4>
      </section>

      <!-- explore section -->
      <section class="col-2">
        <h4>Explore</h4>
      </section>

      <!-- information section -->
      <section class="col-2">
        <h4>Information</h4>
      </section>

      <!-- instagram section -->
      <section class="col-4">
        <h4>Instagram</h4>
      </section>
    </div>

    <!-- row 2 -->
    <div class="row">
      <div class="col-12">PROVA</div>
    </div>
  </div>
</template>

<!-- script -->
<script>
export default {
  data() {
    return {
      address: [
        "382 NE 191st St # 87394 Miami, FL 33179-3899",
        "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)",
        "support@maxcoach.com",
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
</style>
