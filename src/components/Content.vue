<template>
  <section id="content">
    <!-- Spotlight -->
    <div class="spotlight"></div>
    <!-- Comic Book section container -->
    <article class="comics-container container">
      <button class="btn-series">CURRENT SERIES</button>

      <ul>
        <!-- V-for cycle to extract data from all comics -->
        <li v-for="(comic, index) in comics" :key="index">
          <a href="#"><ComicsCard :comic="comic" /></a>
        </li>
      </ul>
      <div class="button-content">
        <button>LOAD MORE</button>
      </div>
    </article>
  </section>
</template>

<script>
import ComicsCard from "../components/ComicsCard.vue";
export default {
  name: "Content",
  props: ["comics"],
  components: {
    ComicsCard,
  },
};
</script>

<style scoped lang="scss">
#content {
  width: 100%;
  background-color: #1c1c1c;
  color: white;
  display: flex;
  align-items: center;
  position: relative;
  padding-top: 300px;
  .spotlight {
    background-image: url("../assets/img/jumbotron.jpg");
    background-position: top center;
    background-size: cover;
    height: 300px;
    width: 100%;
    position: absolute;
    top: 0;
  }
  .comics-container ul {
    display: flex;
    flex-wrap: wrap;
    margin-top: 10px;
    li {
      flex-basis: calc(1200px / 6);
      a {
        color: white;
        &:hover {
          text-decoration: underline;
        }
      }
    }
  }
}
.button-content {
  width: 100%;
  display: flex;
  justify-content: center;
  button {
    background-color: #0476f2;
    color: white;
    font-weight: bold;
    font-size: 12px;
    border: 0;
    padding: 10px 60px;
    margin: 20px;
    cursor: pointer;
    &:hover {
      background-color: white;
      color: #0476f2;
    }
  }
}
.btn-series {
  position: relative;
  top: -20px;
  left: -20px;
  background-color: #0476f2;
  color: white;
  font-weight: bold;
  font-size: 20px;
  border: 0;
  padding: 10px 30px;
  cursor: pointer;
}
</style>