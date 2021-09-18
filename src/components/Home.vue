<template>
  <div class="home">
    <div class="container">
      <div class="picture">
        <span>KUIZ KUIZ KUIZ</span>
        <span>KUIZ KUIZ KUIZ</span>
      </div>
      <div class="content">
        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor 
          in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, 
          sunt in culpa qui officia deserunt mollit anim id est laborum.</span>
      </div>
    </div>
    <button class="button-quiz">
      <a href="#">GO TO QUIZ!</a>
    </button>
    <div class="question-mark">
      <span class="ques1">?</span>
      <span class="ques2">?</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home'
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600&display=swap');

  .home {
    width: 100vw;
    height: 100vh;
    background-color: #B6D8CF;
    display: flex;
    align-content: center;
    justify-content: center;
    position: relative;
  }

  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: inherit;
    width: 70%;
    height: 60%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .picture {
    display: flex;
    flex-direction: column;
    justify-content: start;
    width: 50%;
  }

  .picture span {
    font-size: 70px;
    line-height: 100px;
    font-weight: 600;
    position: relative;
    bottom: 150px;
    left: 50px;
    user-select: none;
    letter-spacing: 2px;
    color: rgb(37, 37, 37);
  }

  .content {
    display: flex;
    width: 50%;
  }

  .content span {
    width: 90%;
    font-size: 24px;
    line-height: 36px;
    color: rgb(56, 56, 56);
  }

  .button-quiz {
    width: 204px;
    height: 51px;
    position: absolute;
    background-color: rgb(31, 167, 172);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.55);
    border-radius: 30px;
    bottom: 220px;
    right: 550px;
    border: none;
    cursor: pointer;
  }

  .button-quiz:hover {
    background-color: rgb(0, 108, 112);
  }

  .button-quiz:active {
    background-color: rgb(0, 108, 112);
    transform: translateY(4px);
  }

  .button-quiz a {
    font-size: 24px;
    font-weight: 600;
    text-decoration: none;
    font-family: 'Rubik', sans-serif;
    color: rgb(216, 216, 216);
  }

  .question-mark {
    display: flex;
    position: relative;
    top: 650px;
    left: 600px;
  }

  .question-mark span {
    font-size: 180px;
  }

  .ques1 {
    position: absolute;
    color: #828282;
    transform: rotate(-7.45deg);
  }

  .ques2 {
    position: absolute;
    color: #333333;
    transform: rotate(20.51deg);
    left: 40px;
  }
</style>
