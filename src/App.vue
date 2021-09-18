<template>
  <div class="app">
    <navbar />
    <home />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import Home from '@/components/Home'

export default {
  name: 'App',
  components: {
    Navbar,
    Home
  }
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
