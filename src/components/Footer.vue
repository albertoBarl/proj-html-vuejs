<template lang="">
  <div class="container">
    <!-- row 1 -->
    <div class="row d-flex">
      <!-- address section -->
      <section class="col-4">
        <h5>Address</h5>
        <p v-for="(item, index) in addressSect">{{ addressSect[index] }}</p>
        <socials />
      </section>

      <!-- explore section -->
      <section class="col-2">
        <h5>Explore</h5>
        <ul v-for="(item, index) in exploreSect" class="list-unstyled">
          <li>
            <a href="/">{{ exploreSect[index] }}</a>
          </li>
        </ul>
      </section>

      <!-- information section -->
      <section class="col-2">
        <h5>Information</h5>
        <ul v-for="(item, index) in informationSect" class="list-unstyled">
          <li>
            <a href="/">{{ informationSect[index] }}</a>
          </li>
        </ul>
      </section>

      <!-- instagram section -->
      <section class="col-4">
        <div class="d-flex align-items-center gap-2">
          <h5 class="">Instagram</h5>
          <a href="/"><span class="instaTag">@maxcoach</span></a>
        </div>
        <div class="d-flex gap-5">
          <div
            class="sPost"
            v-for="(item, index) in instaPosts"
            :class="[index] > 2 ? 'd-none' : ''"
          >
            <img
              :src="`src/assets/images/${instaPosts[index]}`"
              alt="not available"
            />
          </div>
        </div>
      </section>
    </div>

    <!-- row 2 -->
    <div class="row rights">
      <div class="col-12 d-flex justify-content-center">
        &copy; 2020 Maxcoach. All Rights Reserved
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
      instaPosts: [
        "120084500_197897808368764_8114555493043279565_n.jpg",
        "120012142_177596140500760_8623485824101406058_n.jpg",
        "120099363_364334431619755_7198812647386067017_n.jpg",
        "artist-event-01-250x300.jpg",
        "artist-hero-image-02.jpg",
        "artist-course-06-480x480.jpg",
        "artist-hero-image-01.jpg",
        "artist-hero-image-03.png",
        "artist-hero-image-04.jpg",
      ],
    };
  },
};
</script>

<!-- style -->
<style lang="scss" scoped>
@use "../styles/generals.scss" as *;
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;

* {
  line-height: 2.5;
}
.rights {
  padding-top: 100px;
}

.sPost {
  width: 150px;
  img {
    width: 100%;
  }
}

a,
p {
  color: grey;
  text-decoration: none;
}

.instaTag {
  color: $aranciata;
}

.col-12 {
  color: rgb(193, 191, 191);
}
</style>
