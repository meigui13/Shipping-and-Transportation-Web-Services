<template>
  <!-- calc() 能计算的计算表达式里，计算符号两边要有空格
  default-active 高亮
  default-opends 默认展开-->
  <el-menu
      style="width: 200px; min-height: calc(100vh - 50px)"
      :default-active="path"
      router
  >

      <el-menu-item index="/user">
        <i class="el-icon-user"></i>
        <span>用户管理</span>
      </el-menu-item>

      <el-menu-item index="/person">
        <i class="el-icon-user-solid"></i>
        <span>个人信息</span>
      </el-menu-item>

      <el-menu-item index="/wuliu">
        <i class="el-icon-truck"></i>
        <span>物流管理</span>
      </el-menu-item>

  </el-menu>
</template>

<script>
export default {
  name: "",
  data() {
    return {
      user: {},
      path: this.$route.path   // 设置默认高亮的菜单为当前路由
    }
  }
}
</script>

<style scoped>

</style>