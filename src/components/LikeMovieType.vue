<template>
  <div class="LikeMovieType">
    <p>请选择喜欢的专栏</p>
    <ol>
      <li v-for="(h, index) in hoppys" :key="index">
        <input type="checkbox" v-model="flag" :value="h"/>{{ h }}
      </li>
    </ol>
    <ul>
      <li v-for="(h, index) in flag" :key="index">
        {{ h }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "LikeMovieType",
  data() {
    return {
      hoppys: ["科幻", "喜剧", "动漫", "冒险", "科技", "军事", "娱乐", "奇闻"],
      flag: [],
    };
  },
};
</script>

<style scope>
.LikeMovieType {
  margin: 50px auto;
  text-align: center;
}

ol {
  display: flex;
  justify-content: center;
  margin-top: 50px;
}
ol li {
  list-style: none;
  margin: 0 10px;
}
ul {
  margin-top: 50px;
}
ul li {
  margin: 10px;
}
</style>