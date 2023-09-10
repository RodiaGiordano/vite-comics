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
          active: true,
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
          active: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header>
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
  </header>
</template>

<style lang="scss" scoped>
header {
  font-weight: bold;

  .header_wrapper {
    width: 75%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 20px 0;

    ul {
      list-style-type: none;
      display: flex;
      gap: 30px;

      .active {
        color: #0282f9;
        box-shadow: #0282f9 0px 68px 0px -7px;
      }
    }
  }
}
</style>
