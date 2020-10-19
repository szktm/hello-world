<template>
  <div id="title">
  <h1>hi, i'm tomoe</h1>
  </div>
  <div id="nav">
    <router-link to="/">home</router-link> <br>
    <router-link to="/about">about</router-link><br> 
    <router-link to="/work">work</router-link>
  </div>
  <div class="content">
    <router-view/>
  </div>
  
</template>


<style>

#app {
  font-family: 'Rubik', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  padding: 5%;

  
}

#title {
  text-align: left;
  color: #2c3e50;
  padding-right: 100px;

}
#nav {
  width: 15%;
  display: block;
  height: 100vh;
  float: left;
  margin: flex
}

#nav a {
  color: #42b983;
  text-decoration: none;

}

.content {
  margin: auto;

  font-size: 14px

}



</style>
