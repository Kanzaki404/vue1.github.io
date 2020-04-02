<template>
  <div id="app">
    <div id="nav">
      
      <router-link to="/">Home</router-link> |
      <router-link to="/add">Add</router-link> |
      <router-link to="/about">About</router-link>
      
    </div>
    <router-view/>
  </div>
</template>

<style>
*{
  padding: 0;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: url('./assets/bg.jpg');
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

}

#nav {
  padding: 20px;
  float: left;
  background-color:rgba(0, 0, 0, 0.5);
  height: 95vh;
}

#nav a {
  font-weight: bold;
  color: #596168;
  text-decoration-line: none;
  display: block;
}

#nav a.router-link-exact-active {
  color: chartreuse
}
</style>
