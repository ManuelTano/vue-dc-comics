<template>
  <main>
    <div class="container">
      <h2>--> Content goes here</h2>
    </div>

    <div class="shop">
      <div class="container">
        <ul>
          <li>
            <img
              src="../assets/img/buy-comics-digital-comics.png"
              alt="buy-comics-digital-comics"
            /><span>DIGITAL COMICS</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-merchandise.png"
              alt="buy-comics-merchandise"
            /><span>DC MERCHANDISE</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-shop-locator.png"
              alt="buy-comics-shop-locator"
            /><span>SUBSCRIPTION</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-subscriptions.png"
              alt="buy-comics-subscriptions"
            /><span>COMIC SHOP LOCATOR</span>
          </li>
          <li>
            <img
              src="../assets/img/buy-dc-power-visa.svg"
              alt="buy-dc-power-visa" class="visa"
            /><span>DC POWER VISA</span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script >
export default {
  name: "MyMain",
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
 