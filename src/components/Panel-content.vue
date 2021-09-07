<template>
  <section id="panel-content">
    <ul class="container">
      <li>
        <a href="#">
          <img
            src="@/assets/img/buy-comics-digital-comics.png"
            alt="digital-comics"
          />
          digital comics
        </a>
      </li>
      <li>
        <a href="#">
          <img
            src="@/assets/img/buy-comics-merchandise.png"
            alt="comics-merchandise"
          />
          dc merchandise
        </a>
      </li>
      <li>
        <a href="#">
          <img
            src="@/assets/img/buy-comics-subscriptions.png"
            alt="comics-subscriptions"
          />
          subscription
        </a>
      </li>
      <li>
        <a href="#">
          <img
            class="shop-locator"
            src="@/assets/img/buy-comics-shop-locator.png"
            alt="comics-shop-locator"
          />
          comic shop locator
        </a>
      </li>
      <li>
        <a href="#">
          <img
            src="@/assets/img/buy-dc-power-visa.svg"
            alt="buy-dc-power-visa"
          />
          dc power visa
        </a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "Panel-content",
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/general-panel-content-style.scss";
//// Icons style
img {
  width: 40px;
  height: auto;
  margin-right: 10px;
  &.shop-locator {
    width: 28px;
  }
}
</style>