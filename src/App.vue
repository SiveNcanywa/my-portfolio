<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link :to="{ name: 'About' }">About</router-link>
    <router-link :to="{ name: 'Resume' }">Resume</router-link>
    <router-link :to="{ name: 'Skills' }">Skills</router-link>
    <router-link :to="{ name: 'Projects' }">Projects</router-link>
    <router-link :to="{ name: 'Testimonials' }">Testimonials</router-link>
    <router-link :to="{ name: 'Contact' }">Contact</router-link>
  </div>
  <router-view />
</template>
<script>
export default {
  name: "Home",
  components: {},
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  padding: 10px 60px;
  box-sizing: border-box;
  transition: 0.5s;
  z-index: 5;
  opacity: 1;
  background: linear-gradient(0deg, rgba(5, 4, 71, 0.3), rgba(5, 4, 71, 0.3));
}
nav.black {
  background: rgba(0, 0, 0, 0.8);
  height: 80px;
  padding: 10px 50px;
}

nav router-link {
  float: right;
  margin: 0;
  padding: 0;
  display: flex;
}
nav router-link {
  list-style: none;
  margin-top: 25px;
  line-height: none;
  font-size: 18px;
  color: white;
  padding: 5px 15px;
  text-decoration: none;
  text-transform: uppercase;
  transition: 1s;
  text-shadow: 0 0 10px #000;
}
</style>
