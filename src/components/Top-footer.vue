<template>
  <section id="top-footer">
    <div class="container">
      <div class="row">
        <div class="col">
          <h4><a href="#">dc comics</a></h4>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h4><a href="#">shop</a></h4>
          <ul>
            <li><a href="#">Shop dc</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="col">
          <h4><a href="#">dc</a></h4>
          <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="col">
          <h4><a href="#">sites</a></h4>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <figure class="logo-bg"></figure>
    </div>
  </section>
</template>

<script>
export default {
  name: "Top-footer",
};
</script>

<style scoped lang="scss">
#top-footer {
  height: 45vh;
  background-image: url("../assets/img/footer-bg.jpg");
  background-position: top;
  background-size: cover;
  background-repeat: no-repeat;
  .container {
    display: flex;
    justify-content: space-between;
    .logo-bg {
      height: 45vh;
      width: 600px;
      background-image: url("../assets/img/dc-logo-bg.png");
      background-repeat: no-repeat;
      background-position: center;
    }
  }
}

#top-footer .container .row {
  display: flex;
  justify-content: space-evenly;
  .col {
    margin-top: 40px;
    margin-right: 30px;
    h4 {
      margin: 10px 0;
      a {
        text-decoration: none;
        text-transform: uppercase;
        font-size: 22px;
        color: white;
        &:hover {
          text-decoration: underline;
        }
      }
    }
  }
  ul li a {
    font-size: 14px;
    color: #959595;
    &:hover {
      text-decoration: underline;
    }
  }
}
</style>