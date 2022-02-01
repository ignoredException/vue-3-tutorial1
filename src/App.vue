<template>
  <body>  
    <header>
      <img alt="Vue logo" src="./assets/logo.png">
    </header>
    <div class="center">
      <div class="nav">
        <a class="active" href="./">Home</a>
        <div class="dropdown">
          <button class="dropdown-button">Dropdown</button>
          <div class="dropdown-content">
            <a href="">Drop 1</a>
            <a href="">Drop 2</a>
            <a href="">Drop 3</a>
          </div>
        </div>
        <a href="">Navbar 3</a>
        <a href="">Navbar 4</a>
        <a href="">Navbar 5</a>
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
    background-color: lightgray;
    color: white;
}

.nav a.active {
    background-color: darkcyan;
    color: white;
}

.dropdown {
  position: relative;
  display: inline-block;
  float: left;
}

.dropdown-button {
  background-color: gray;
  color: white;
  border: none;
  padding: 14px 16px;
  font-size: 20px;
  text-align: center;
  text-decoration: none;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: gray;
  min-width: 100px;
  font-size: 20px;
  text-align: center;
  text-decoration: none;
}

.dropdown-content a:hover {
  background-color: lightgray;
  min-width: 74%;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.dropdown:hover .dropdown-button {
   background-color: lightgray;
}

</style>
