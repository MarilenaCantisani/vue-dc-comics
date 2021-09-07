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
@import "@/assets/scss/general-style/style.scss";
</style>
