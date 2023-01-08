<template>
  <div id="app">
    <h1 class="title">hello world</h1>
    <FruitStore></FruitStore>
    <!-- <hr /> -->
    <LikeMovieType></LikeMovieType>
  </div>
</template>

<script>
import LikeMovieType from "./components/LikeMovieType.vue";
import FruitStore from "./components/FruitStore.vue";

export default {
  name: "App",
  components: {FruitStore, LikeMovieType},
};
</script>

<style scoped>
.title {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
