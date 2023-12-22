<script>
import Logo from './components/Logo.vue';
import Navbar from './components/Navbar.vue';
import AppHeader from './components/AppHeader.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    Logo,
    Navbar,
    Footer
  }
}
</script>
<template>
  <div id="app">
    <AppHeader />
    <Footer />


  </div>
</template>
