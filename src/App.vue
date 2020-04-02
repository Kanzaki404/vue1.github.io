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
<script>
export default {
  name: 'App'
}
</script>
<style>
@import url('https://fonts.googleapis.com/css?family=Orbitron&display=swap');
*{
  padding: 0;
  margin: 0;
   background-color: #2a3439;
}
#app {
  
  font-family: 'Orbitron', sans-serif, monospace;
  letter-spacing: 2px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
  /* background-image: url('./assets/bg.jpg');
  height: 100vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover; */

  background-color: #2a3439;
background-size: cover;
}

#nav {
  padding: 20px;
  float: left;
  color: rgb(116, 116, 116);

}

#nav a {
  font-weight: bold;
  color: #687077;
  text-decoration-line: none;
  display: block;
}

#nav a.router-link-exact-active {
  color: chartreuse
}
</style>
