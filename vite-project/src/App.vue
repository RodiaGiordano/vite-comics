<script>
import appHeader from "./components/appHeader.vue";

import appFooter from "./components/appFooter.vue";

import appMain from "./components/appMain.vue";

export default {
  components: { appHeader, appFooter, appMain },
};
</script>

<template>
  <div class="container">
    <appHeader />
  </div>
</template>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

.container {
  padding: 30px 150px;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
