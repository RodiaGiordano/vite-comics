<script>
export default {
  data() {
    return {
      cards: [
        {
          pic: "buy-comics-digital-comics.png",
          pic_text: "DIGITAL COMICS",
        },
        {
          pic: "buy-comics-merchandise.png",
          pic_text: "DC MERCHANDISE",
        },
        {
          pic: "buy-comics-subscriptions.png",
          pic_text: "SUBSCRIPTION",
        },
        {
          pic: "buy-comics-shop-locator.png",
          pic_text: "COMIC SHOP LOCATOR",
        },
        {
          pic: "buy-dc-power-visa.svg",
          pic_text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="footer_top">
      <div v-for="(card, index) in cards" class="card">
        <img :src="'../../public/vue-dc-comics-1/img/' + card.pic" alt="" />
        <span>{{ card.pic_text }}</span>
      </div>
    </div>

    <div class="footer_middle"></div>

    <div class="footer_bottom"></div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  font-size: 0.7rem;
  color: white;
}
.footer_top {
  background-color: #0282f9;
  padding: 50px 0;

  display: flex;
  justify-content: center;
  align-items: center;
  gap: 70px;

  .card {
    display: flex;
    align-items: center;
    gap: 10px;

    img {
      width: 50px;
    }
  }
}
</style>
