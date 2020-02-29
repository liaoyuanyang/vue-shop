<template>
  <div>
    <el-button type="info" @click="loginout">退出</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    loginout() {
      window.sessionStorage.clear(); // 清空token
      this.$router.push("/login"); // 跳转到登录页
    }
  }
}
</script>

<style lang="less" scoped>
</style>