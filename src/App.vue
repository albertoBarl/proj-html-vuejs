<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
import eventscount from "./components/elements/eventscount.vue";

export default {
  components: {
    // main components
    Header,
    Footer,
    Main,
    // others
    eventscount,
  },
  data() {
    return {
      navbar: [
        {
          section: "Home",
          dropdowns: [
            "MaxCoach Education",
            "Course Portal",
            "Distance Learning",
            "Multimedia Pedagogy",
            "Modern Scrolling",
            "Remote Training",
            "Healt Coaching",
            "Gym Coaching",
            "Business",
            "Artist",
            "Kitchen Coach",
            "Motivation",
            "Dancing",
            "Guitar",
            "Yoga",
            "Photography",
            "Personal Finance",
            "Sales Coaching",
            "Mental Therapy",
          ],
        },
        {
          section: "Pages",
          dropdowns: [
            "Start Here",
            "Succes Story",
            "About me",
            "About us 01",
            "About us 02",
            "About us 03",
            "Contact me",
            "Contact us",
            "Purchase Guide",
            "Privacy Policy",
            "Terms of Service",
          ],
        },
        {
          section: "Courses",
          dropdowns: [
            "Course Gride 01",
            "Course Gride 02",
            "Course Gride 03",
            "Membership Levels",
            "Become a Teacher",
            "Profile",
            "Checkout",
            "Single Layout",
          ],
        },
        { section: "Features", dropdowns: ["Events", "Zoom Meetings"] },
        {
          section: "Blog",
          dropdowns: ["Blog Grid", "Blog Masonry", "Blog Classic", "Blog List"],
        },
        {
          section: "Shop",
          dropdowns: [
            "Shop Left Sidebar",
            "Shop Right Sidebar",
            "Cart",
            "Wishlist",
            "Single Product",
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <div class="eventscount">
    <eventscount />
  </div>
  <div class="header">
    <Header :navbar="navbar" :key="index" />
  </div>
  <div class="main">
    <Main />
  </div>
  <div class="footer">
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
@use "./styles/generals.scss" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/partials/variables" as *;

// .eventscount {
// }
.header {
  background-color: $wall;
  position: fixed;
  width: 100%;
  z-index: 4;
  // top: 0;
}

.footer {
  background-color: $d-wall;
}
</style>
