<template>
<header>
  <img alt="Vue logo" src="./assets/main_gif.gif" height="220">
  <Header msg="Welcome to My First Vue App"/>
  <h1> </h1>
</header>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Header from './components/Header.vue'


export default {
  name: 'App',
  components: {
    Header,
    Navbar
	}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: auto;
}

.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 12px;
  font-family: inherit;
}
</style>
