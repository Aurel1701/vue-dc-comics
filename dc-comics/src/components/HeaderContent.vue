<template>
  <section>
    <div class="current-series">current series</div>
    <div class="cards-box">
      <div v-for="(card, index) in cards" :key="index" class="cards">
        <img :src="card.thumb" />
        <h3>{{ card.series }}</h3>
      </div>
    </div>
    <button>load more</button>
  </section>
</template>

<script>
export default {
  name: "HeaderContent",
  props: {
    cards: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
section {
  background-color: black;
  position: relative;
  text-transform: uppercase;
  color: whitesmoke;
  text-align: center;
  font-size: 13px;
  font-weight: bold;
  .current-series {
    position: absolute;
    margin: -20px 250px;
    width: 200px;
    background-color:blue;
    padding: 10px 10px;
    font-size: 18px;
  }
  .cards-box {
    width: 65%;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;

    .cards {
      margin-top: 30px;
      width: 200px;
      padding: 10px;

      img {
        width: 100%;
        &:hover {
          opacity: 50%;
        }
      }
      h3 {
        margin-top: 5px;
      }
    }
  }
  button {
    background-color: blue;
    border: none;
    padding: 15px 50px;
    margin: 20px auto;
    color: white;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 15px;
    cursor: pointer;

    &:hover {
      background-color: lightgreen;
    }
  }
}
</style>