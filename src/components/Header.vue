<template>
  <header class="container">
    <figure><img id="logo" src="@/assets/img/dc-logo.png" alt="logo" /></figure>
    <nav>
      <ul class="uppercase">
        <li><a href="#">characters</a></li>
        <li><a id="active" href="#">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">videos</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
//// General header style
header {
  height: 12vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  //* List style
  nav ul {
    display: flex;
    li a {
      padding: 10px;
      color: black;
      font-size: 14px;
      font-weight: 600;
      &:hover {
        color: #0476f2;
        border-bottom: 1px solid #0476f2;
      }
    }
  }
}
//* Header logo style
#logo {
  width: 60px;
}
</style>
