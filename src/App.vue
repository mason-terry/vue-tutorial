<template>
  <div class="app">
    <a href='http://localhost:8080/#/'>Home</a>
    <a href='http://localhost:8080/#/profile'>Profile</a>
    <a href='http://localhost:8080/#/login'>Login</a>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
.app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
a {
  text-decoration: none;
  margin: 20px;
  font-weight: 800;
  font-size: 2rem;
}
</style>
