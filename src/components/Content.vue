<template>
  <section id="content">
    <div class="spotlight"></div>
    <article class="comics-container">
      <ul>
        <li>
          <ComicsCard />
        </li>
      </ul>
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
  display: flex;
  align-items: center;
  .spotlight {
    background-image: url("../assets/img/jumbotron.jpg");
    background-position: top center;
    background-size: cover;
    height: 300px;
    width: 100%;
  }
}
</style>