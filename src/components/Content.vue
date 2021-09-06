<template>
  <section id="content">
    <div class="text-content container">Content goes here</div>
  </section>
</template>

<script>
export default {
  name: "Content",
};
</script>

<style scoped lang="scss">
#content {
  width: 100%;
  height: 15vh;
  background-color: #1c1c1c;
  display: flex;
  align-items: center;
  //* Text content style
  .text-content {
    color: white;
    font-size: 24px;
    font-weight: bold;
  }
}
</style>