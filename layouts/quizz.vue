<template>
  <div>
      <Nuxt />
  </div>
</template>

<script>
  export default {
    // les propriétés de la page vont ici
    name : 'quizz'
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500&display=swap');

  html {
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

    body {
    font-family: "Monsterrat", sans-serif;
    height: 100vh;
    background: url('~assets/images/back.jpg');
    background-repeat: no-repeat;
    background-size: cover;
  }

  *,
  *::before,
  *::after {
    box-sizing: border-box;
    margin: 0;
  }
