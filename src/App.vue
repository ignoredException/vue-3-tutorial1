<template>
  <body>  
    <header>
      <img alt="Vue logo" src="./assets/logo.png">
    </header>
    <div class="center">
      <div class="nav">
        <a class="active" href="home-site.vue">Home</a>
        <a href="calculator-site.vue">Calculator</a>
      </div>        
    </div>
    <Home />
  </body>
</template>

<script>
import Home from './components/home-component.vue'

export default {
  name: 'App',
  components: {
    Home,
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
  background: transparent;
  margin: 50px;
  padding: 10px;
}

 body {
  background-color: white;
  background-position: middle;
  background-size: cover;
  background-attachment: fixed;
  background-image: url("https://i.pinimg.com/originals/0b/87/b8/0b87b83c20672d122f3fea5e220bcec0.jpg");
}

.center {
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: none;
}

.nav {
    background-color: gray;
    overflow: lightgray;    
    width: 87%;
    padding: 0px;
    background-image: none;
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
