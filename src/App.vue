<template>
  <div id="title">
  <h1>hi, i'm tomoe</h1>
  <p> beep boop this site is under construction </p>
  </div>
  <div id="nav">
    <router-link to="/">home</router-link> <br>
    <router-link to="/about">about</router-link><br> 
    <router-link to="/work">work</router-link>
  </div>
  <router-view/>
  
</template>

<style>
#app {
  font-family: 'Rubik', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  padding-left: 100px;
  padding-top: 50px;

  
}
#title {
  text-align: left;
  color: #2c3e50;
  padding-right: 100px;

}
#nav {
  align-content: left;
  text-align: left;
  padding-right: 100px;
  width: 20%;
  height: 100%;
  float: left;
  display: inline-block
  
}

#nav a {
  color: #42b983;
  text-decoration: none;

}


</style>
