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
//// General footer style
#bottom-footer {
  background-color: #303030;
  height: 12vh;
  .container .row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 12vh;
  }
}
//// Footer button style
#bottom-footer button {
  border-radius: 0;
  border: 1px solid #0476f2;
  padding: 12px 10px;
  background-color: #303030;
  cursor: pointer;
  a {
    text-decoration: none;
    text-transform: uppercase;
    color: white;
    font-weight: bolder;
  }
  &:hover {
    background-color: #0476f2;
  }
}
//// Style social section of the footer
//* Style text social section
#bottom-footer .container .row .social-section {
  height: 12vh;
  display: flex;
  align-items: center;
  span a {
    text-transform: uppercase;
    text-decoration: none;
    color: #0476f2;
    font-weight: bold;
    padding: 0 25px;
    &:hover {
      text-shadow: 0 0 2px #0476f2;
    }
  }
}
//* Style icons social section
#bottom-footer .container .row .social-section a img {
  width: 28px;
  margin: 0 6px;
  &:hover {
    transform: scale(1.1);
  }
}
</style>