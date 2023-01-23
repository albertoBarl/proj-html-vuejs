<template lang="">
  <div class="container">
    <!-- row 1 -->
    <div class="row d-flex text-white">
      <!-- address section -->
      <section class="col-4">
        <h4>Address</h4>
        <p v-for="(item, index) in addressSect">{{ addressSect[index] }}</p>
        <div class="socialsLogos d-flex gap-4 mt-4">
          <ul class="list-unstyled" v-for="(item, index) in socialLogos">
            <li>
              <a href="/"><i :class="`${socialLogos[index].icona}`"></i></a>
            </li>
          </ul>
        </div>
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
      socialLogos: [
        { type: "facebook", icona: "fab fa-facebook-square" },
        { type: "twitter", icona: "fab fa-twitter" },
        { type: "instagram", icona: "fab fa-instagram" },
        { type: "linkedin", icona: "fab fa-linkedin" },
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

h4 {
  margin-bottom: 20px;
  color: black;
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

i {
  font-size: 34px;
  color: grey;
}
a,
p {
  color: grey;
}
</style>
