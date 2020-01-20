<template>
  <div class="top-nav">
    <el-menu
      :default-active="activeIndex2"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b"
    >
      <el-menu-item index="0">
        <img
          style="background-size:cover;"
          height="60"
          src="https://juvou.bluearp.com/images/logo.png"
          alt
        />
      </el-menu-item>
      <el-menu-item index="1">
        <span>处理中心</span>
      </el-menu-item>
      <el-menu-item index="2">
        <span>我的工作台</span>
      </el-menu-item>
      <el-menu-item index="3">
        <span>消息中心</span>
      </el-menu-item>
      <el-menu-item index="4">
        <span>订单管理</span>
      </el-menu-item>
      <div class="last-option">
        <div class="user-info">
          <span>管理员:Acvount</span>
        </div>
      </div>
    </el-menu>
  </div>
</template>
<script>
export default {
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
  }
};
</script>

<style>
.top-nav > ul,
.top-nav > ul li {
  background-color: #2a303e !important;
  color: rgba(255, 255, 255, 0.75) !important;
}
html,
body {
  overflow: hidden;
}
.el-menu.el-menu--horizontal {
  border-bottom: 0;
}
.top-nav .el-menu-item.is-active > span {
  color: #2a303e !important;
  background-color: #fff !important;
  border-radius: 25px;
  display: inline-block;
  line-height: 27px;
  width: 85px;
  text-align: center;
}
.top-nav .el-menu-item.is-active {
  border-bottom: 3px solid #c1dbf6 !important;
}
.top-nav .last-option {
  display: inline-block;
  float: right;
  height: 60px;
  margin-right: 60px;
  outline: none
}
.top-nav .last-option .user-info {
  display: inline-block;
  margin: 0 auto;
  transform: translate(0%,80%);
}
</style>