<template lang="html">
  <div id="register-vue">

    <div class="form-wrapper">
      <el-form class="">

        <el-form-item label="아이디">
          <el-input placeholder="아이디를 입력해주세요"></el-input>
        </el-form-item>

        <el-form-item label="비밀번호">
          <el-input type="password" placeholder="비밀번호를 입력해주세요"></el-input>
        </el-form-item>

        <el-form-item>
          <el-button type="danger">Query</el-button>
        </el-form-item>

      </el-form>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Register'
}
</script>

<style lang="css" scoped>
#register-vue {
  width: 100%;
  height: 100%;
}
</style>
