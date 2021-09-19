<template>
  <div class="navbar">
    <div class="wrapper">
      <div class="left">
        <router-link to="/"><img src="@/assets/kuiz.png" alt="" class="logo"></router-link>
        <div class="quiz">
          <router-link to="/quiz" class="quiz-text">QUIZ</router-link>
        </div>
      </div>
      <div class="right">
        <div class="login">
          <router-link to="/login" class="login-text">Login</router-link>
        </div>
        <div class="signup">
          <router-link to="/register" class="signup-text">Sign up</router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navbar'
}
</script>

<style scoped>
  .navbar {
    width: 100%;
    color: #000;
    font-size: 14px;
    position: fixed;
    top: 0;
    z-index: 999;
    background: linear-gradient(to top, transparent 0%, rgb(0, 0, 0, 0.15) 50%);
  }

  .wrapper {
    padding: 0px 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100px;
  }

  .left {
    display: flex;
    align-items: center;
  }

  .left img {
    width: 148px;
    height: 82px;
    margin-right: 50px;
  }

  .quiz-text {
    font-size: 24px;
    text-decoration: none;
    color: rgb(88, 88, 88);
    letter-spacing: 2px;
    font-weight: 600;
    position: relative;
  }

  .quiz-text:hover {
    color: rgb(54, 54, 54);
  }

  .quiz-text:before {
    content: "";
    position: absolute;
    height: 0.15em;
    width: 0%;
    background-color: rgb(0, 115, 119);
    bottom: -0.1em;
    transition: 0.3s ease-in-out;
  }

  .quiz-text:hover:before {
    width: 100%;
  }

  .right {
    display: flex;
    align-items: center;
  }

  .login-text, .signup-text {
    font-size: 24px;
    text-decoration: none;
    color: rgb(88, 88, 88);
    letter-spacing: 2px;
    font-weight: 500;
    position: relative;
  }

  .login-text:hover {
    color: rgb(54, 54, 54);
  }

  .login-text:before {
    content: "";
    position: absolute;
    height: 0.15em;
    width: 0%;
    background-color: rgb(0, 115, 119);
    bottom: -0.1em;
    transition: 0.3s ease-in-out;
  }

  .login-text:hover:before {
    width: 100%;
  }

  .signup {
    margin: 0 60px;
    padding: 8px 15px;
    border: 1px solid black;
    border-radius: 25px;
    cursor: pointer;
  }

  .signup:hover {
    background-color: rgb(0, 115, 119);
    border: 1px solid rgb(0, 115, 119);;
  }

  .signup:hover a {
    color: #fff;
  }

</style>
