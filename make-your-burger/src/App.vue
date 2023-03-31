<template>
  <div>
    <Navbar :logo="src" :alt="appName"/>
    <div>
      <router-view/>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import Navbar from './components/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Footer,
  },
  data() {
    return {
      src: '/img/logo.png',
      appName: 'Make Your Burger'
    }
  },
}
</script>

<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.main-container {
  margin: 50px;
  min-height: 250px;
}
h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
