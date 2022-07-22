<template>
  <div id="app">
    <MyHeader />
    <MyMain />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";
import MyFooter from "./components/MyFooter.vue";

export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },
};
</script>

<style lang="scss">

#app {

}

body {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
  margin: 0 auto; 
  height: 100vh;
  background-color: black;
}

.container {
  margin: 0 auto;
  width: 1200px;
}

img {
  max-width: 100%;
  height: auto;
}

</style>
