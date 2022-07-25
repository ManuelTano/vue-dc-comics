<template>
  <main>
    <div class="container">
      <h2>--> Content goes here</h2>
    </div>

    <div class="shop">
      <div class="container">
        <ul>
          <li v-for="(shop, index) in shops" :key="index">
            <img :src="shop.src" :alt="shop.text" />
            <span> {{ shop.text }}</span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script >
export default {
  name: "MyMain",
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

img {
  width: 15%;
}

span {
  color: $white;
  margin-left: 10px;
}

.visa {
  width: 50px;
}
</style>
 