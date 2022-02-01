<template>
  <header>
    <img alt="Vue logo" src="./assets/logo.png">
  </header>
  <body>
    <div class="nav">
      <a class="active" href="calculator-site.vue">Calculator</a>
      <a href="calculator-site.vue">Test</a>
    </div>    
    <Home />
    <Calculator />
  </body>
</template>

<script>
import Home from './components/home-component.vue'
import Calculator from './components/calculator-component.vue'

export default {
  name: 'App',
  components: {
    Home,
    Calculator,
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
  margin-top: 60px;
}

header {
  background-color: lightgray;
  size: 100%;
  margin: 0px;
  padding: 0px;
}

body {
  background-color: white;
}

.nav body {
    background-color: deepskyblue;
}

.nav {
    background-color: gray;
    overflow: hidden;
}

.nav a {
    float: left;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 20px;
}

.nav a:hover {
    background-color: gray;
    color: black;
}

.nav a.active {
    background-color: darkcyan;
    color: white;
}

</style>
