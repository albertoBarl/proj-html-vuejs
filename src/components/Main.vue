<template lang="">
  <jumbotron />
  <artistcoachSect />
</template>
<script>
import jumbotron from "./elements/jumbotron.vue";
import artistcoachSect from "./elements/artistcoachSect.vue";

export default {
  components: {
    jumbotron,
    artistcoachSect,
  },
};
</script>
<style lang="scss" scoped>
@use "../styles/generals.scss" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;
</style>
