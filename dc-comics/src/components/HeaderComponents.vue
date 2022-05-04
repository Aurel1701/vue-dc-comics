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
             <li v-for="(item, index) in navbar" :key="index">
                 <a :href="item.url">{{item.text}}</a>
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
  data (){
    return{
      navbar: [
        {
          id: "1",
          text: "characters",
          url: "#",
        },
        {
          id: "2",
          text: "movies",
          url: "#",
        },
        {
          id: "3",
          text: "tv",
          url: "#",
        },
        {
          id: "4",
          text: "games",
          url: "#",
        },
        {
          id: "5",
          text: "collectibles",
          url: "#",
        },
        {
          id: "6",
          text: "videos",
          url: "#",
          },
        {
          id: "7",
          text: "fans",
          url: "#",
        },
        {
          id: "8",
          text: "news",
          url: "#",
        },
        {
          id: "9",
          text: "shop",
          url: "#",
        },
        {
          id: "10",
          text: "comics",
          url: "#",
        }
    ],



    }
    
  }
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
        display: flex;
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
          a {
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



