<script>
import Logo from './components/Logo.vue';
import Navbar from './components/Navbar.vue';
import AppHeader from './components/AppHeader.vue';
import Footer from './components/Footer.vue';
import AppMain from './components/AppMain.vue';
import jumbotron from './components/jumbotron.vue';




export default {
  name: 'App',
  components: {
    AppHeader,
    Logo,
    Navbar,
    AppMain,
    jumbotron,
    Footer
  }
}
</script>
<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <Footer />


  </div>
</template>
