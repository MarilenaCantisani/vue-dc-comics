<template>
  <section id="bottom-footer">
    <div class="container">
      <div class="row">
        <div class="col">
          <button><a href="#">Sign-up now!</a></button>
        </div>
        <div class="col social-section">
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
@import "@/assets/scss/bottom-footer/bottom-footer.scss";
</style>