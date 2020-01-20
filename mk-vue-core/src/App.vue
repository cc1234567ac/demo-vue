<template>
  <div id="app">
    <top-nav></top-nav>

    <el-row :gutter="20">
      <el-col :span="3">
        <left-nav></left-nav>
      </el-col>
      <el-col :span="21">
        <div class="grid-content bg-purple">ac</div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import leftNav from "@/components/common/left-nav";
import topNav from "@/components/common/top-nav";
export default {
  name: "app",
  components: {
    topNav,
    leftNav
  }
};
</script>

<style scoped>
</style>>
