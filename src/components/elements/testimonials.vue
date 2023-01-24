<template lang="">
  <div class="container-fluid">
    <div class="pCenter">
      <h2>Testimonials</h2>
      <h3>Why do people love me?</h3>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@use "../../styles/generals.scss" as *;
@use "../../styles/partials/mixins" as *;
@use "../../styles/partials/variables" as *;

.pCenter {
  display: flex;
  flex-direction: column;
  align-items: center;
  h3 {
    width: 75%;
    text-align: center;
    font-weight: 500;
  }
  h2 {
    font-family: cursive;
    font-style: italic;
    font-size: 40px;
    color: $cielo;
  }
}
</style>
