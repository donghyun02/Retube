<template lang="html">
  <div id="register-vue">
    <router-link to="/" class="title">Retube</router-link>
    <div class="form-wrapper">
      <el-form class="form">

        <el-form-item label="이름">
          <el-input class="input" placeholder="이름을 입력해주세요" v-model="name"></el-input>
        </el-form-item>

        <el-form-item label="아이디">
          <el-input class="input" placeholder="아이디를 입력해주세요" v-model="username"></el-input>
        </el-form-item>

        <el-form-item label="비밀번호">
          <el-input class="input" type="password" placeholder="비밀번호를 입력해주세요" v-model="password"></el-input>
        </el-form-item>

        <el-form-item label="비밀번호 확인">
          <el-input class="input" type="password" placeholder="비밀번호를 확인해주세요" v-model="passwordCheck"></el-input>
        </el-form-item>

        <el-form-item>
          <el-button type="danger">회원가입</el-button>
        </el-form-item>

      </el-form>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Register',
  data() {
    return {
      name: '',
      username: '',
      password: '',
      passwordCheck: ''
    }
  }
}
</script>

<style lang="css" scoped>
#register-vue {
  width: 100%;
  height: 100%;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.title {
  color: #F56C6C;
  text-decoration: none;
  font-size: 48px;
  font-weight: 900;
}

.form-wrapper {
  width: 30%;
}

</style>
