<template>
  <nav>
    <router-link to="/" id="logo-url">
      <img id="logo" :src="logo" :alt="alt">
    </router-link>
    <router-link to="/">Home</router-link>
    <router-link to="/pedidos">About</router-link>
  </nav>
</template>

<script>
  export default {
    name: 'Navbar',
    props: ['logo', 'alt']
  }
</script>

<style scoped>
  nav {
    display: flex;
    justify-content: flex-end;
    align-content: center;
    background: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
  }

  #logo-url {
    margin: auto;
    margin-left: 0;
  }

  #logo {
    width: 40px;
    height: 40px;
  }

  nav a {
    margin: 12px;
    color: #fcba03;
    text-decoration: none;
    transition: .5s;
  }

  nav a:hover {
    color: #fff;
  }
</style>