<template>
  <div class="headSearch">
    <div :gutter="20">
      <el-col :span="6">
        <div class="slogan">豆瓣读书</div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeadSearch",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.headSearch {
  width: 1040px;
}
</style>
