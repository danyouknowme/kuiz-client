<template>
  <div class="navbar">
    <div class="wrapper">
      <div class="left">
          <img src="@/assets/kuiz.png" alt="" class="logo">        
          <div class="quiz">
            <a href="#">QUIZ</a>
          </div>
      </div>
      <div class="right">
        <div class="login">
          <a href="#">Login</a>
        </div>
        <div class="signup">
          <a href="#">Sign up</a>
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

  .quiz a {
    font-size: 24px;
    text-decoration: none;
    color: rgb(88, 88, 88);
    letter-spacing: 2px;
    font-weight: 600;
    position: relative;
  }

  .quiz a:hover {
    color: rgb(54, 54, 54);
  }

  .quiz a:before {
    content: "";
    position: absolute;
    height: 0.15em;
    width: 0%;
    background-color: rgb(0, 115, 119);
    bottom: -0.1em;
    transition: 0.3s ease-in-out;
  }

  .quiz a:hover:before {
    width: 100%;
  }

  .right {
    display: flex;
    align-items: center;
  }

  .login a, .signup a {
    font-size: 24px;
    text-decoration: none;
    color: rgb(88, 88, 88);
    letter-spacing: 2px;
    font-weight: 500;
    position: relative;
  }

  .login a:hover {
    color: rgb(54, 54, 54);
  }

  .login a:before {
    content: "";
    position: absolute;
    height: 0.15em;
    width: 0%;
    background-color: rgb(0, 115, 119);
    bottom: -0.1em;
    transition: 0.3s ease-in-out;
  }

  .login a:hover:before {
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
