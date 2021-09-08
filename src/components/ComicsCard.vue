<template>
  <div class="card">
    <figure>
      <img class="comic-img" :src="comic.thumb" :alt="comic.series" />
    </figure>
    <figcaption class="uppercase">{{ comic.series }}</figcaption>
  </div>
</template>

<script>
export default {
  name: "ComicsCard",
  props: ["comic"],
};
</script>

<style scoped lang="scss">
</style>