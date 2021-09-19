<template>
  <div class="app">
    <router-view />
  </div>
</template>

<script>

export default {
  name: 'App',
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600&display=swap');

  html, body {
    margin: 0 !important;
    padding: 0 !important;
  }

 .app {
   margin: 0;
   overflow: hidden;
   font-family: 'Rubik', sans-serif;
 }
</style>
