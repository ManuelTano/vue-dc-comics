<template>
  <div id="app">
    <MyHeader />
    <MyMain :cards="cards" />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";
import MyFooter from "./components/MyFooter.vue";
import json from "./dc-comics.json";

export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },
  data() {
    return {
      cards: json,
    };
  },
};
</script>

<style lang="scss">
@import "./assets/sass/_style.scss";
</style>
