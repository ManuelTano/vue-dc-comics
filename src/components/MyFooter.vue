<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="firstcol">
            <h4>DC COMICS</h4>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h4>SHOP</h4>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>

          <div class="secondocol margin">
            <h4>DC</h4>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshop</a></li>
              <li><a href="#">CPSC Cerificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>

          <div class="thirdcol margin">
            <h4>SITES</h4>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>

        <div class="col-image">
          <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg" />
        </div>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container">
        <div class="row">
          <div class="col">
            <div class="button">
              <h3><a href="#" class="white">SIGN UP NOW!</a></h3>
            </div>
          </div>
          <div class="col">
            <div class="col center"><h3 class="blue">FOLLOW US</h3></div>
            <div class="col center"><img src="../assets/img/footer-facebook.png" alt="footer-facebook"></div>
            <div class="col center"><img src="../assets/img/footer-twitter.png" alt="footer-twitter"></div>
            <div class="col center"><img src="../assets/img/footer-youtube.png" alt="footer-youtube"></div>
            <div class="col center"><img src="../assets/img/footer-pinterest.png" alt="footer-pinterest"></div>
            <div class="col center"><img src="../assets/img/footer-periscope.png" alt="footer-periscope"></div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MyFooter",
};
</script>

<style scoped lang="scss">
@import "../assets/sass/vars";


footer {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.row {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.col {
  display: flex;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
  color: $gray;
}

.margin {
  margin-left: 25px;
}

h4 {
  color: $white;
}

.col-image {
  overflow: hidden;
  text-align: end;
}

img {
  width: 80%;
  margin-top: -50px;
  margin-bottom: -50px;
}

.footer-bottom {
  background-color: #303030;
  display: flex;
  justify-content: space-between;
  padding-top: 20px;
  padding-bottom: 20px;
}
.button {
  border: 2px solid $blue;
  padding: 0 10px;
  cursor: pointer;
}

.white {
  color: $white;
}

.blue {
  color: $blue;
}

.col img {
  height: 35px;
  width: 35px;
  margin: 0;
  padding: 0 10px;
  cursor: pointer;
}

.center {
  justify-content: center;
  align-items: center;
}
</style>