<template>
  <section>
    <div class="shop-zone">
        <SectionShop />
      <ul>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          <span>digital comics</span>
        </li>
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="" />
          <span>dc merchandise</span>
        </li>
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
          <span>subscription</span>
        </li>
        <li>
          <img
            class="shop-locator"
            src="../assets/img/buy-comics-shop-locator.png"
            alt=""
          />
          <span>comic shop locator</span>
        </li>
        <li>
          <img class="visa" src="../assets/img/buy-dc-power-visa.svg" alt="" />
          <span>dc power visa</span>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
import SectionShop from "@/components/ContentShop";
export default {
  name: "ContentShop",
  components: {
    SectionShop,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
section {
  background-color:rgba(2, 130, 249, 1);
  text-transform: uppercase;
  .shop-zone {
    margin: 0px 200px;
    ul {
      display: flex;
      justify-content: space-around;
      align-items: center;
      text-transform: uppercase;
      li {
        display: flex;
        align-items: center;
        color: white;
        list-style: none;
        padding: 20px;
        cursor: pointer;

        img {
          width: 40px;
          margin-right: 15px;
        }
        &:hover {
          text-decoration: underline;
        }
      }
    }

    .shop-locator {
      width: 28px;
    }
    .visa {
      width: 40px;
    }
  }
}
</style>