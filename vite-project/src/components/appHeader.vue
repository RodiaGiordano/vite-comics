<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <main>
    <div class="header_wrapper">
      <img src="/vue-dc-comics-1/img/dc-logo.png" alt="" />
      <ul>
        <li>CHARACTER</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </main>
</template>

<style lang="scss" scoped>
main {
  font-weight: bold;
  font-size: 0.6rem;
  img {
    width: 80px;
  }

  .header_wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;

    ul {
      list-style-type: none;
      display: flex;
      gap: 30px;
    }
  }
}
</style>
