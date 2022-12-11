<template>
  <div class="login">
    <h1>Login</h1>

    <div class="input_row">
      <label for="id">아이디: </label>
      <input type="text" id="id" v-model="user.userid" />
    </div>
    <div class="input_row">
      <label for="password">비밀번호: </label>
      <input type="password" id="password" v-model="user.password" /><br />
    </div>
    <div>
      <button>로그인</button>
      <!-- <router-link to="/SignUp">&nbsp;&nbsp;sign up</router-link> -->
    </div>
  </div>
</template>

<script>
export default {
  name: "Login",

  data() {
    return {
      user: {
        userid: "",
        password: "",
      },
    };
  },
};
</script>
<style scoped></style>
