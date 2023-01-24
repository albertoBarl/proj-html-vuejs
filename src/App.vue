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
            { label: "MaxCoach Education", status: "hot" },
            { label: "Course Portal", status: null },
            { label: "Distance Learning", status: "hot" },
            { label: "Multimedia Pedagogy", status: null },
            { label: "Modern Scrolling", status: null },
            { label: "Remote Training", status: null },
            { label: "Healt Coaching", status: null },
            { label: "Gym Coaching", status: null },
            { label: "Business", status: null },
            { label: "Artist", status: null },
            { label: "Kitchen Coach", status: null },
            { label: "Motivation", status: null },
            { label: "Dancing", status: null },
            { label: "Guitar", status: null },
            { label: "Yoga", status: null },
            { label: "Photography", status: null },
            { label: "Personal Finance", status: null },
            { label: "Sales Coaching", status: "new" },
            { label: "Mental Therapy", status: "new" },
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
            {
              theName: "Single Layout",
              insideDrop: [
                "Free Course",
                "Sticky Features Bar",
                "Standard Sidebar",
                "No Sidebar",
              ],
            },
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
    <Header :navbar="navbar" />
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
  // position: fixed;
  // width: 100%;
  // top: 0;
}

.footer {
  background-color: $d-wall;
}
</style>
