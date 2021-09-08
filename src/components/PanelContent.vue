<template>
  <section id="panel-content">
    <ul class="container d-flex j-content-around a-items-center">
      <li v-for="(item, index) in itemsPanel" :key="index">
        <a href="#">
          <img :src="item.url" :alt="item.text" />
          {{ item.text }}
        </a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "Panel-content",
  data() {
    return {
      itemsPanel: [
        {
          url: require("@/assets/img/buy-comics-digital-comics.png"),
          text: "digital comics",
        },
        {
          url: require("@/assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise",
        },
        {
          url: require("@/assets/img/buy-comics-subscriptions.png"),
          text: "subscription",
        },
        {
          url: require("@/assets/img/buy-comics-shop-locator.png"),
          text: "comic shop locator",
        },
        {
          url: require("@/assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
//// Variable
@import "@/assets/scss/GeneralStyle/_vars.scss";
//// General panel content style
@import "@/assets/scss/PanelContent/PanelContent.scss";
//// Icons style
img {
  width: 40px;
  height: auto;
  margin-right: 10px;
}
</style>