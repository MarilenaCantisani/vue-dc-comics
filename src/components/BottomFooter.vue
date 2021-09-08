<template>
  <section id="bottom-footer">
    <div class="container">
      <div class="row d-flex a-items-center j-content-between">
        <!-- Button "Sign-up" -->
        <div class="col">
          <button class="clickable"><a href="#">Sign-up now!</a></button>
        </div>
        <!-- Social section -->
        <div class="col social-section d-flex a-items-center">
          <span><a href="#">follow us</a></span>
          <a href="#"
            ><img src="@/assets/img/footer-facebook.png" alt="fb"
          /></a>
          <a href="#"
            ><img src="@/assets/img/footer-twitter.png" alt="twitter"
          /></a>
          <a href="#"
            ><img src="@/assets/img/footer-youtube.png" alt="youTube"
          /></a>
          <a href="#"
            ><img src="@/assets/img/footer-pinterest.png" alt="pinterest"
          /></a>
          <a href="#"
            ><img src="@/assets/img/footer-periscope.png" alt="periscope"
          /></a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Bottom-footer",
};
</script>

<style scoped lang="scss">
//// Variable
@import "@/assets/scss/GeneralStyle/_vars.scss";
//// Style Footer
@import "@/assets/scss/BottomFooter/BottomFooter.scss";

//// General footer style
#bottom-footer {
  background-color: $grey;
  height: 12vh;
  .container .row {
    height: 12vh;
  }
}
</style>