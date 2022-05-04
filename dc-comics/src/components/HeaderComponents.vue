<template>
  <header>
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
    <div class="logo2">
      <img class="img-logo2" src="@/assets/img/jumbotron.jpg" alt="logo2" />
    </div>
  </header>
  
</template>

<script>
export default {
  name: "HeaderComponents",
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
          text: "comics",
          url: "#",
        },
        {
          id: "3",
          text: "movies",
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
          text: "tv",
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
          

          &:hover {
            color: black;
            border-bottom: 5px solid blue;
          }
          a {
            padding-right: 15px;
            text-decoration: none;
            color: black;
          }.logo2{
            height: 400px;
            background-size: cover;
          }img-logo2{
            height: 400px;
            max-width: 100%;
          }
        }
      }
    }
  }
}
</style>



