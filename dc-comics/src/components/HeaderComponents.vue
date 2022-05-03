<template>
  <header>
    <SiteLogo />
    <div class="header-container">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="logo" />
      </div>
      <nav class="header-navbar">
        <ul>
          <li>
            <h3>CHARACTERS</h3>
            <h3>COMICS</h3>
            <h3>MOVIES</h3>
            <h3>TV</h3>
            <h3>GAMES</h3>
            <h3>COLLECTIBES</h3>
            <h3>VIDEOS</h3>
            <h3>FANS</h3>
            <h3>NEWS</h3>
            <h3>SHOP</h3>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
import SiteLogo from "@/components/HeaderComponents";
export default {
  name: "HeaderComponents",
  components: {
    SiteLogo,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
header {
  .header-container {
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    align-items: center;
    .logo {
      margin: 15px 10px;
    }
    .header-navbar {
      ul {
        li {
          display: flex;
          padding: 15px;
          list-style: none;
          text-transform: uppercase;
          font-weight: bold;
          cursor: pointer;

          &:hover {
            color: black;
            border-bottom: 5px solid blue;
          }
          h3 {
            padding-right: 15px;
            text-decoration: none;
            color: black;
          }
        }
      }
      .content-goes {
        height: 150px;
        background-color: black;
        .h2{
            color: greenyellow;
        }
      }
    }
  }
}
</style>



