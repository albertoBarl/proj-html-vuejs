<template lang="">
  <jumbotron />
</template>
<script>
import jumbotron from "./elements/jumbotron.vue";

export default {
  components: {
    jumbotron,
  },
};
</script>
<style lang="scss" scoped>
@use "../styles/generals.scss" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;
</style>
