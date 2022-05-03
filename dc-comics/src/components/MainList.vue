<template>
  <main>
    <MainSection />
    <div class="footer-left">
      <ul>
        <li><h4>DC COMICS</h4></li>
        <li><a href="#">Characters</a></li>
        <li><a href="#">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">Tv</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">News</a></li>
      </ul>

      <ul>
        <li><h4>SHOP</h4></li>
        <li><a href="#">Shop DC</a></li>
        <li><a href="#">Shop DC Collectibles</a></li>
      </ul>

      <ul>
        <li><h4>DC</h4></li>
        <li><a href="#">Terms Of Use</a></li>
        <li><a href="#">Privacy policy (New)</a></li>
        <li><a href="#">Ad Choices</a></li>
        <li><a href="#">Advertising</a></li>
        <li><a href="#">Jobs</a></li>
        <li><a href="#">Subscriptions</a></li>
        <li><a href="#">Talent Workshops</a></li>
        <li><a href="#">CPSC Certificates</a></li>
        <li><a href="#">Ratings</a></li>
        <li><a href="#">Shop Help</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>

      <ul>
        <li><h4>SHOP</h4></li>
        <li><a href="#">DC</a></li>
        <li><a href="#">MAD Magazine</a></li>
        <li><a href="#">DC Kids</a></li>
        <li><a href="#">DC Universe</a></li>
        <li><a href="#">DC Power Visa</a></li>
      </ul>
    </div>

    <div class="footer-right-logo">
      <img src="../assets/img/dc-logo-bg.png" alt="" />
    </div>
  </main>
</template>

<script>
import MainSection from "@/components/MainList";
export default {
  name: "MainList",
  components: {
    MainSection,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
main {
  height: 450px;
  display: flex;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;
  
  .footer-left {
    display: flex;
    padding: 70px;
    margin-left: 20px;

    ul {
      margin: 0 15px 10px 30px;

      li {
        list-style: none;
        margin-left: 20px;
        line-height: 30px;

        h4 {
          font-size: 18px;
          color: white;
          text-transform: uppercase;
        }
        a {
          text-decoration: none;
          color: grey;

          &:hover {
            color: whitesmoke;
          }
        }
      }
    }
  }
  .footer-right-logo {
    margin: 10px 200px;

    img {
      margin: -90px 0;
    }
  }
}
</style>