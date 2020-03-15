<template>
  <div id="app">
    <div>
      <b-navbar class="navbar" id="nav" toggleable="lg" fixed="top">
        <b-navbar-brand  class="navbar-brand" href="#home">
          <h1>Alif</h1>
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" class="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item class="nav-item" href="#home" right>Home</b-nav-item>
            <b-nav-item class="nav-item" href="#profile" right>Profile</b-nav-item>
            <b-nav-item class="nav-item" href="#services" right>Services</b-nav-item>
            <b-nav-item class="nav-item" href="#education" right>Education</b-nav-item>
            <b-nav-item class="nav-item" href="#language" right>Language</b-nav-item>
            <b-nav-item class="nav-item" href="#contact" right>Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
        </b-navbar>
    </div>
    <Profile msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import Profile from './components/Profile.vue'

export default {
  name: 'App',
  components: {
    Profile
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Habibi');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.navbar {
  background-color: #D3D0D0;
}
.nav-item {
  padding: 10px;
  font-weight: bold;
  font-family: 'Habibi';
}
h1 {
  font-size: 2rem;
  text-align: center;
}
</style>
