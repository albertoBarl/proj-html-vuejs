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
          <ul v-for="(item, index) in navbar" class="list-unstyled">
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
