<template>
  <div id="app">
    <!--//// Header -->
    <Header />
    <!--//// Main -->
    <main>
      <!-- Main content section -->
      <Content />
      <!-- Content panel section -->
      <Panel-content />
    </main>
    <!--//// Footer -->
    <footer>
      <!-- Footer information section -->
      <Top-footer />
      <!-- Footer section social profiles -->
      <Bottom-footer />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import PanelContent from "./components/Panel-content.vue";
import TopFooter from "./components/Top-footer.vue";
import BottomFooter from "./components/Bottom-footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    PanelContent,
    TopFooter,
    BottomFooter,
  },
};
</script>

<style lang="scss">
//// RESET
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Work Sans", sans-serif;
}
//// UTILITY
//* General
.container {
  width: 1200px;
  margin: 0 auto;
}
img {
  max-width: 100%;
  height: auto;
}
ul li {
  list-style-type: none;
  a {
    text-decoration: none;
  }
}
#active {
  color: #0476f2;
  border-bottom: 1px solid #0476f2;
}
//* Text style
.uppercase {
  text-transform: uppercase;
}
</style>
