<template>
  <Navbar
    :logo="logo_src"
    :alt="app_name"
  />
  <router-view/>
  <Footer />
</template>

<script>
  import Navbar from './components/Navbar.vue';
  import Footer from './components/Footer.vue';

  export default {
    components: {
      Navbar,
      Footer
    },
    data() {
      return {
        logo_src: '/img/logo.png',
        app_name: 'Make Your Burguer'
      }
    }
  }
</script>


<style>
  * {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
    font-family: Helvetica;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    margin-bottom: 30px;
    font-size: 42px;
    color: #222;
    text-align: center;
  }
</style>
