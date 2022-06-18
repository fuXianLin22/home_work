<template>
  <div id="app">
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
  components: { FruitStore, LikeMovieType },
};
</script>

<style>
</style>
