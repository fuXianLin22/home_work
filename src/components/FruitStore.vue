<template>
  <div class="fruit">
    <ul>
      <li>欢迎光临我们的水果店</li>
      <li>苹果10￥/斤，折扣(8折)</li>
      <li>请输入要购买的斤数 <input type="text" v-model="num" /></li>
      <li>
        <button @click="checkOut">结账买单~</button>
      </li>
      <li>
        结账单：总价： {{ total }}￥ 折后价： {{ discount }}￥ 省了：
        {{ saveMoney }}￥
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FruitStore",
  data() {
    return {
      num: 1,
    };
  },
  computed: {
    total() {
      return this.num * 10;
    },
    discount() {
      return (this.total / 10) * 8;
    },
    saveMoney() {
      return this.total - this.discount;
    },
  },
  methods: {
    checkOut() {
      this.num = 1;
      alert("结账成功，欢迎再次光临");
    },
  },
};
</script>

<style scope>
* {
  margin: 0;
  padding: 0;
}
.fruit {
  /* width: 500px; */
  height: 300px;
  margin: 0 auto;
}
.fruit ul li {
  list-style: none;
  height: 60px;
  line-height: 60px;
  text-align: center;
  border: 1px solid #999;
}
</style>