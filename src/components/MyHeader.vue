<template>
  <header>
    <div class="container">
      <nav>
        <div class="image">
          <img src="../assets/img/dc-logo.png" alt="dc-logo" />
        </div>
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#" class="active">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
};
</script>

<style>
header {
  background-color: white;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
}

ul {
  display: flex;
  align-items: center;
}

ul li {
  height: 100%;
  font-weight: bold;
  display: flex;
  align-items: center;
  cursor: pointer;
}

a {
  color: grey;
  padding: 0px 10px;
  text-decoration: none;
}

.active {
  color: #0282F9;
}
</style>