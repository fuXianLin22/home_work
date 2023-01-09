<template>
  <div id="app">
    <h1 class="title">hello world</h1>
    <button @click="btn">链接</button>
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
  methods: {
    btn() {
      // window.open('http://10.73.194.156:18099/api/download/u=763387957,687177997&fm=253&fmt=auto&app=138&f=JPEG_20230109173657.png', '_blank')
      window.open('https://www.baidu.com')
    }
  }
};
</script>

<style scoped>
.title {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
