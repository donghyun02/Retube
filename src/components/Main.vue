<template lang="html">
  <div id="main-vue">
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
      <el-menu-item index="1">
        <span class="title">Retube</span>
      </el-menu-item>
      <el-menu-item class="form-wrapper">
        <el-form class="form">
          <el-input class="input" placeholder="" v-model="query"></el-input>
        </el-form>
      </el-menu-item>
      <el-menu-item>
        <router-link to="/login">로그인</router-link>
      </el-menu-item>
      <el-menu-item>
        <router-link to="/register">회원가입</router-link>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'Main',
  data () {
    return {
      activeIndex: '1',
      query: ''
    }
  }
}
</script>

<style lang="css" scoped>
.title {
  color: #F56C6C !important;
  text-decoration: none;
  font-size: 32px;
  font-weight: 900;
}

.form {
  width: 500px;
}
</style>
