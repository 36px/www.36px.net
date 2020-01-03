<style scoped>
.logo-text {
  display: inline-block;
  padding: 0px;
  margin: 0px;
  margin-left: 10px;
  margin-right: 10px;
  color: #aaa;
  font-size: 20px;
  font-weight: bolder;
}

.logo-image {
  display: inline-block;
  background-image: url(https://release.bitwormhole.com/static/36px.net/www/36px-skew.png);
  background-size: 50px 50px;
  background-repeat: no-repeat;
  width: 50px;
  height: 50px;
}
</style>

<template>
  <div class="hello">
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
    >
      <el-menu-item index="1">首页</el-menu-item>

      <el-submenu index="2">
        <template slot="title">产品</template>
        <el-menu-item index="2-1">这不是网盘</el-menu-item>
      </el-submenu>

      <el-submenu index="3">
        <template slot="title">技术</template>
        <el-menu-item index="3-1">分布式数据仓库</el-menu-item>
      </el-submenu>

      <el-submenu index="4">
        <template slot="title">服务</template>
        <el-menu-item index="4-1">技术咨询</el-menu-item>
        <el-menu-item index="4-2">方案设计</el-menu-item>
        <el-submenu index="4-3">
          <template slot="title">软件开发</template>
          <el-menu-item index="4-1">iOS App 开发</el-menu-item>
          <el-menu-item index="4-2">Android App 开发</el-menu-item>
          <el-menu-item index="4-3">微信小程序开发</el-menu-item>
          <el-menu-item index="4-3">HTML5 Web 开发</el-menu-item>
          <el-menu-item index="4-3">Java Web App 开发</el-menu-item>
          <el-menu-item index="4-3">Windows 桌面 App 开发</el-menu-item>
          <el-menu-item index="4-3">Linux 桌面 App 开发</el-menu-item>
        </el-submenu>
      </el-submenu>

      <el-menu-item index="5">最新动态</el-menu-item>
      <el-menu-item index="6">关于</el-menu-item>

      <el-menu-item index="7">
        <template>
          <div class="logo-text">三十六像素App加工厂</div>
          <div class="logo-image"></div>
        </template>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: "PageHeader",
  props: {
    msg: String
  },

  data() {
    return {
      activeIndex: "1"
    };
  },

  methods: {
    handleSelect() {}
  }
};
</script>
