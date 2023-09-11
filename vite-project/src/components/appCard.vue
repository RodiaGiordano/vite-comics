<script>
export default {
  props: { card: Object },
};
</script>

<template>
  <div class="card">
    <img :src="card.thumb" alt="" />
    <span>{{ card.series }}</span>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6 - 20px);
  font-size: 0.6rem;

  img {
    width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    object-position: 0% 0%;
  }
}
</style>
