<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <main>
    <div class="jumbo">
      <img src="../../public/vue-dc-comics-1/img/jumbotron.jpg" alt="" />
    </div>
    <div class="main_wrapper"></div>
  </main>
</template>

<style lang="scss" scoped>
main {
  .jumbo {
    height: 400px;

    img {
      height: 100%;
      width: 100%;
      object-fit: cover;
      object-position: 0% 0%;
    }
  }
  .main_wrapper {
    padding: 50px 0;

    width: 75%;
    margin: auto;
    color: white;

    display: flex;
    align-items: center;

    font-size: 1.5rem;
  }
}
</style>
