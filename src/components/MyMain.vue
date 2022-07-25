<template>
  <main>
    <div id="cards">
      <div class="container">
        <MyCards :cards="cards" />
      </div>
    </div>

    <div class="shop">
      <div class="container">
        <ul>
          <li v-for="(shop, index) in shops" :key="index" class="shopping">
            <img :src="shop.src" :alt="shop.text" />
            <span> {{ shop.text }}</span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script >
import MyCards from "./MyCards.vue";
export default {
  name: "MyMain",
  components: { MyCards },
  props: {
    cards: Array,
  },
  data() {
    return {
      shops: [
        {
          text: "Digital Comics",
          src: require("../assets/img/buy-comics-digital-comics.png"),
        },
        {
          text: "DC Merchandise",
          src: require("../assets/img/buy-comics-merchandise.png"),
        },
        {
          text: "Subscription",
          src: require("../assets/img/buy-comics-subscriptions.png"),
        },
        {
          text: "Shop Location",
          src: require("../assets/img/buy-comics-shop-locator.png"),
        },
        {
          text: "DC Power Visa",
          src: require("../assets/img/buy-dc-power-visa.svg"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/sass/vars";

h2 {
  color: $white;
}

.shop {
  background-color: $blue;
  padding: 25px;
}

ul {
  display: flex;
  justify-content: center;
  list-style-type: none;
  padding: 0;
  margin: 0;
  cursor: pointer;
}

ul li {
  align-items: center;
  display: flex;
}

.shopping img {
  width: 40px;
  height: 50px;
}

.shopping {
  margin-left: 20px;
}

span {
  color: $white;
  margin-left: 10px;
}

.visa {
  width: 50px;
}

#cards {
  padding-top: 40px;
  padding-bottom: 40px;
}
</style>
 