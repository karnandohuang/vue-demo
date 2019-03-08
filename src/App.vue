<template>
  <div id="app">
    <router-link to="/">
      <img src="~assets/blibli-logo.png" alt="blibli logo">
    </router-link>
    <div>
      <router-link to="/contact-us" class="button">Contact Us</router-link>
    </div>
    <div class="content">
      <router-view/>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .button {
    background-color: aliceblue;
    margin: 5px;
    padding: 5px;
    border-radius: 5px;
    text-decoration: none;
    color: black;
    font-weight: bold;
  }

  .content {
    padding-top: 20px;
  }
</style>
