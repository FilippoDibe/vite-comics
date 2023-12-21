<script>
import Logo from './Logo.vue';
import Navbar from './Navbar.vue';

export default {
    name: 'AppHeader',
    components: {
        Logo,
        Navbar
    }
}
</script>

<template>
    <header class="app-header">
        <Logo />
        <Navbar />
    </header>
</template>
  

  
<style scoped>
.app-header {
    /* Stili per l'header */

    display: flex;
    justify-content: space-evenly;
    /* align-items: center; */
    padding-top: 1rem;
    background-color: white;
    position: absolute;
    top: 0;
    width: 100%;
    box-sizing: border-box;
}
</style>
  