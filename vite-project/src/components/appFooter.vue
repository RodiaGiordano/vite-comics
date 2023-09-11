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

      linkFooter: [
        {
          nameList: "DC COMICS",
          links: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },

        {
          nameList: "SHOP",
          links: ["Shop DC", "Shop DC Collectibles"],
        },

        {
          nameList: "DC",
          links: [
            "Terms Of Use",
            "Privacy policy (New)",
            "Ad Choices",
            "Advertising",
            "jobs",
            "Subscriptions",
            "Talent Workshops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },

        {
          nameList: "SITES",
          links: [
            "DC",
            "MAD magazine",
            "DC Kids",
            "DC Universe",
            "DC power Visa",
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="footer_top">
      <section>
        <div v-for="(card, index) in cards" class="card">
          <img :src="'../../public/vue-dc-comics-1/img/' + card.pic" alt="" />
          <span>{{ card.pic_text }}</span>
        </div>
      </section>
    </div>

    <div class="footer_middle">
      <section>
        <div class="listLinks" v-for="nameList in linkFooter">
          <h3>{{ nameList.nameList }}</h3>

          <ul>
            <li v-for="list in nameList.links">
              {{ list }}
            </li>
          </ul>
        </div>
      </section>
    </div>

    <div class="footer_bottom">
      <section>
        <div class="sing_up">SIGN-UP NOW!</div>
        <div class="ft_icons">
          <ul>
            <li class="follow_us">FOLLOW US</li>

            <li>
              <img
                src="../../public/vue-dc-comics-1/img/footer-facebook.png"
                alt=""
              />
            </li>

            <li>
              <img
                src="../../public/vue-dc-comics-1/img/footer-twitter.png"
                alt=""
              />
            </li>
            <li>
              <img
                src="../../public/vue-dc-comics-1/img/footer-youtube.png"
                alt=""
              />
            </li>
            <li>
              <img
                src="../../public/vue-dc-comics-1/img/footer-pinterest.png"
                alt=""
              />
            </li>
            <li>
              <img
                src="../../public/vue-dc-comics-1/img/footer-periscope.png"
                alt=""
              />
            </li>
          </ul>
        </div>
      </section>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer > * {
  color: white;
  padding: 50px 0;

  ul {
    list-style-type: none;
  }
}

.footer_top {
  background-color: #0282f9;

  section {
    width: 70%;
    margin: auto;

    display: flex;
    justify-content: center;
    align-items: center;
    gap: 70px;
  }

  .card {
    width: calc(100% / 5 - 10px);
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    font-size: 0.5rem;

    img {
      width: 40px;
      aspect-ratio: 1;

      object-fit: contain;
    }
  }
}

.footer_middle {
  background-image: url("../../public/vue-dc-comics-1/img/dc-logo-bg.png"),
    url("../../public/vue-dc-comics-1/img/footer-bg.jpg");
  background-size: 30%, cover;

  background-position: 75%;
  background-repeat: no-repeat;

  height: calc(100% / 2);

  section {
    width: 75%;
    height: 100%;
    margin: 0 auto;

    display: flex;
    align-content: flex-start;
    flex-direction: column;

    flex-wrap: wrap;
    gap: 30px;

    .listLinks {
      ul {
        padding-top: 10px;
        color: #6c717a;

        li {
          font-size: 0.9rem;
          line-height: 1.3rem;
        }
      }
    }
  }
}

.footer_bottom {
  background-color: #303030;
  height: calc(100% / 5);

  section {
    width: 75%;
    height: 100%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .sing_up {
      border: 3px solid #0282f9;
      padding: 20px;
    }

    ul {
      display: flex;
      align-items: center;
      gap: 20px;

      img {
        width: 50px;
      }

      .follow_us {
        color: #0282f9;
        font-weight: bold;
        font-size: 1.3rem;
      }
    }
  }
}
</style>
