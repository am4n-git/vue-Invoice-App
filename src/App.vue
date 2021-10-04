<template>
  <div >
    <div id="app flex">
      <Navigation />
      <div class="app-content flex flex-column">
          <router-view/>
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue"
export default {
  component:{
    Navigation
  }
}
</script>



<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap");
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #141625;
  min-height: 100vh;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
