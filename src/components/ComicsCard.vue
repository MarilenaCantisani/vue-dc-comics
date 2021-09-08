<template>
  <div class="card">
    <!-- Image of the comic -->
    <figure class="img-comic">
      <img :src="comic.thumb" :alt="comic.series" />
    </figure>
    <!-- Title of the comic -->
    <figcaption class="title-comic uppercase">{{ comic.series }}</figcaption>
  </div>
</template>

<script>
export default {
  name: "ComicsCard",
  props: ["comic"],
};
</script>

<style scoped lang="scss">
//// Comic card style
.card {
  margin-bottom: 50px;
  margin-right: 20px;
  .title-comic {
    font-size: 14px;
    margin-top: 10px;
  }
  .img-comic {
    height: 180px;
    overflow: hidden;
  }
}
</style>