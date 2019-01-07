<template>
  <div class="nav-list">
    <ul>
      <li v-for="(item,index) in NavList" :key="index" :index="(index).toString()">
        <img :src="item.imgUrl" alt>
        <span v-text="item.title"></span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      NavList: [
        {
          title: "生活缴费",
          imgUrl: require("../assets/money.png")
        },
        {
          title: "缴费记录",
          imgUrl: require("../assets/rule.png")
        },
        {
          title: "物业服务",
          imgUrl: require("../assets/reseve.png")
        },
        {
          title: "个人中心",
          imgUrl: require("../assets/myself.png")
        }
      ]
    };
  }
};
</script>

<style scoped>
.nav-list {
  width: 100%;
  position: fixed;
  bottom: 0;
  background-color: #ebebeb;
}
ul {
  height: 75px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
li {
  font-size: 14px;
  display: grid;
  text-align: -webkit-center;
}
img {
  margin-bottom: 5px;
  width: 30px;
  height: 30px;
}
</style>
