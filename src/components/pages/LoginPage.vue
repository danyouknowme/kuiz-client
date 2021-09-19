<template>
  <div class="login">
    <div class="container">
      <div class="text">
        Login
      </div>
      <div class="form">
        <form action="">
          <div class="username">
            <label for="username">Username</label>
            <input type="text" name="username" id="" placeholder="Type your username">
          </div>
          <div class="password">
            <label for="password">Password</label>
            <input type="text" name="password" id="" placeholder="Type your password">
          </div>
        </form>
      </div>
      <div class="button">
        <a class="btn">LOGIN</a>
      </div>
      <div class="signup">
        <span>Doesn't have an account ?<router-link to='register' class="signup-text">SIGN UP HERE!</router-link></span>
      </div>
    </div>
  </div>
</template>

<script>

  export default {
    name: 'LoginPage',
  }
</script>

<style scoped>
  html, body {
    margin: 0 !important;
    padding: 0 !important;
  }

  .login {
    width: 100vw;
    height: 100vh;
    background-image: linear-gradient(#B6D8CF, rgb(192, 192, 192));
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .container {
    width: 30%;
    height: 60%;
    background-color: #fff;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: start;
  }

  .text {
    font-size: 38px;
    font-weight: 600;
    margin: 40px 0;
  }

  .button {
    width: 400px;
    height: 40px;
    background-image: linear-gradient(to bottom, rgb(31, 167, 172), rgb(70, 175, 180));
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.55);
    border-radius: 30px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .button:hover {
    background-image: linear-gradient(to top, rgb(8, 124, 128), rgb(130, 193, 196));
  }

  .button:active {
    background-color: rgb(0, 108, 112);
    transform: translateY(2px);
  }

  a {
    font-size: 18px;
    font-weight: 500;
    color: #fff;
  }

  .form {
    width: 70%;
    height: 50%;
  }

  .username {
    display: flex;
    flex-direction: column;
    margin: 40px 0;
  }

  .password {
    display: flex;
    flex-direction: column;
  }

  input {
    border: 0;
    outline: 0;
    background: transparent;
    border-bottom: 1px solid grey;
    margin: 10px 0;
    font-size: 16px;
    font-family: inherit;
  }

  .signup {
    width: 70%;
    display: flex;
    justify-content: center;
    margin-top: 40px;
  }

  .signup-text {
    margin-left: 10px;
    color: rgb(145, 18, 18);
    text-decoration: none;
    position: relative;
  }

  .signup-text:hover {
    color: rgb(107, 54, 54);
  }
</style>
