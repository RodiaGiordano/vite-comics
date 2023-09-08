<script>
export default {
  data() {
    return {
      listLinks: [
        {
          linkText: "CHARACTER",
          active: false,
        },
        {
          linkText: "COMICS",
          active: false,
        },

        {
          linkText: "MOVIES",
          active: false,
        },

        {
          linkText: "TV",
          active: false,
        },

        {
          linkText: "GAMES",
          active: false,
        },

        {
          linkText: "COLLECTIBLES",
          active: false,
        },

        {
          linkText: "VIDEOS",
          active: false,
        },

        {
          linkText: "FANS",
          active: false,
        },

        {
          linkText: "NEWS",
          active: false,
        },

        {
          linkText: "SHOP",
          active: true,
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="header_wrapper">
      <img src="/vue-dc-comics-1/img/dc-logo.png" alt="" />
      <ul>
        <li
          v-for="(link, index) in listLinks"
          :class="link.active ? 'active' : ''"
        >
          {{ link.linkText }}
        </li>
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
