<template>
  <div class="topTabs">
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
    >
    <el-menu-item index="1">豆瓣</el-menu-item>
    <el-menu-item index="2">读书</el-menu-item>
    <el-menu-item index="3">电影</el-menu-item>
    <el-menu-item index="4">音乐</el-menu-item>
    <el-menu-item index="5">同城</el-menu-item>
    <el-menu-item index="6">小组</el-menu-item>
    <el-menu-item index="7">阅读</el-menu-item>
    <el-menu-item index="8">FM</el-menu-item>
    <el-menu-item index="9">时间</el-menu-item>
    <el-menu-item index="10">豆品</el-menu-item>
    <el-menu-item index="11" class="right">下载豆瓣客户端</el-menu-item>
    <el-menu-item index="12" class="right">登录/注册</el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: "TopTabs",
  data() {
    return {
      activeIndex: "1",
      activeIndex2: "1"
    };
  },
  methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.right{
  float: right;
}
.el-menu-item{
  height: 30px;
  line-height: 30px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
