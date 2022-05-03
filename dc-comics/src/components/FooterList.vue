<template>
  <section>
    <div class="contacts">
        <FooterSection />
      <div class="sign-up">
        <button><a href="#">SING-UP NOW!</a></button>
      </div>

      <div class="icons-zone">
        <span>FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png" alt="" />
        <img src="../assets/img/footer-twitter.png" alt="" />
        <img src="../assets/img/footer-youtube.png" alt="" />
        <img src="../assets/img/footer-pinterest.png" alt="" />
        <img src="../assets/img/footer-periscope.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
import FooterSection from "@/components/FooterList";
export default {
  name: "FooterList",
  components: {
    FooterSection,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
.contacts {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: black;
  .sign-up {
    margin-left: 100px;
    button {
      background-color: rgb(48, 48, 48);
      border: none;
      border: 2px solid rgba(2, 130, 249, 1);
      padding: 15px;
      margin: 20px;
      a {
        text-transform: uppercase;
        font-weight: bold;
        text-decoration: none;
        color: white;
        font-size: 15px;
      }
      &:hover {
        background-color: black;
      }
    }
  }

  .icons-zone {
    display: flex;
    justify-content: space-around;
    margin-right: 300px;

    img {
      padding: 10px;
      width: 50px;
      height: 50px;
      &:hover {
        background-color:black ;
        border-radius: 50px 50px;
      }
    }
    span {
      color:rgba(2, 130, 249, 1);
      font-weight: bold;
      font-size: 20px;
      text-transform: uppercase;
      margin: 15px 10px;
      cursor: pointer;
      &:hover {
        border-bottom: 1px solid rgba(2, 130, 249, 1);
      }
    }
  }
}
</style>