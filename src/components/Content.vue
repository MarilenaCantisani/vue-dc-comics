<template>
  <section id="content">
    <!-- Spotlight -->
    <div class="spotlight bg-style w-100"></div>
    <!-- Comic Book section container -->
    <article class="comics-container container">
      <button class="btn-series clickable">CURRENT SERIES</button>
      <ul class="d-flex f-wrap">
        <!-- V-for cycle to extract data from all comics -->
        <li v-for="(comic, index) in comics" :key="index">
          <a href="#"><ComicsCard :comic="comic" /></a>
        </li>
      </ul>
      <div class="btn-content d-flex j-content-center w-100">
        <button class="clickable">LOAD MORE</button>
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
//// Variable
@import "@/assets/scss/GeneralStyle/_vars.scss";
////General style of the section content
@import "@/assets/scss/ContentStyle/ContentStyle.scss";
////Button style
@import "@/assets/scss/ContentStyle/ButtonStyle.scss";
</style>