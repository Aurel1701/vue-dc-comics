<template>
  <div class="content-goes">
    <Goes />
    <h2 class="title-goes">--> Content goes here >--</h2>
  </div>
</template>

<script>
import Goes from "@/components/HeaderContent";
export default {
  name: "HeaderContent",
  components: {
    Goes,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/img/sass/_common.scss";
.content-goes {
  height: 150px;
  background-color: black;
  display: flex;
  align-items: center;
  padding-left: 200px;
}.title-goes{
    color: white;
    font-size: 25px;
}
</style>