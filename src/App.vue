<script >

import Logo from './components/Logo.vue';
import Navbar from './components/Navbar.vue';
import AppHeader from './components/AppHeader.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    Logo,
    Navbar
  }
}
</script>

<template>
  <div id="app">
    <AppHeader />
    <!-- il resto della tua app va qui -->
  </div>
</template>

<style lang="scss" scoped>
#app {
  width: 100vw;
  /* Imposta la larghezza massima al 100% */
  margin: 0;
  /* Elimina i margini */
  padding: 0;
  /* Elimina i padding, se presenti */
  box-sizing: border-box;
  /* Assicurati che padding e border siano inclusi nella larghezza */
}

/* Stile aggiuntivo per assicurarsi che tutto sia attaccato al bordo */
html,
body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
}
</style>
