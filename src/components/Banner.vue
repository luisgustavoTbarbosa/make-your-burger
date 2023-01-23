<template>
  <div id="main-banner">
    <h1>Make Your Burguer</h1>
  </div>
</template>

<script>
  export default {
    name: 'Banner'
  }
</script>

<style scoped>
  #main-banner {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    height: 500px;
    background: url('/public/img/burger.jpg') center;
    background-size: cover;
  }

  #main-banner h1 {
    padding: 20px 40px;
    background: #222;
    color: #fff;
    font-size: 60px;
    text-align: center;
  }
</style>