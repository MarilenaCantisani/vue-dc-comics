<template>
  <header class="container d-flex j-content-between a-items-center">
    <!-- Logo -->
    <figure><img id="logo" src="@/assets/img/dc-logo.png" alt="logo" /></figure>
    <!-- Nav bar -->
    <nav>
      <ul class="uppercase d-flex">
        <li v-for="(navItem, index) in navItems" :key="index">
          <a :href="navItem.url" :class="{ active: navItem.current }">
            {{ navItem.text }}
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navItems: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
//// Variable
@import "@/assets/scss/GeneralStyle/_vars.scss";
//// General style header
@import "@/assets/scss/HeaderStyle/HeaderStyle.scss";
//* Header logo style
#logo {
  width: 60px;
}
</style>
