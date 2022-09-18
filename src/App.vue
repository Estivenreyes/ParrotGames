<script setup>

</script>

<template>
  <header>
    <div class="nav">
      <img alt="Parrot logo" class="logo" src="./assets/img/logo.svg"/>
      <nav class="navbar" id="navegation menu">
      </nav>
    </div>   
  </header>

  <section class="landing">
    <figure class="landing--svg">
      <img class="landing--logo" src="./assets/img/logoLanding.svg" alt="landingLogo">
    </figure>
    <div class="landing__content">
      <h2 class="landing--h2">Welcome to</h2>
      <h1 class="landing--h1">Parrot Games</h1>
      <p class="landing--text">Parrot Games is a video game distribution company with a social component, 
        where our users can interact with others, criticize and review their favorite video games.</p>
    </div>
  </section>

  <main>
    <TheWelcome />
  </main>
</template>

<style lang="scss">
  $blue: #1569DB;
  $gray: #2E2E2E;
  $nav: #232323;

*{
  box-sizing: border-box;
}

body{
  margin: 0;
}

.nav {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  position: fixed;
  background: rgba(35, 35, 35, 0.8);
  
  padding: 23px;
  color: #000000;
  z-index: 10;
}

.landing{
  background-image: url("../src/assets/img/landingPage.png");
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;

  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 485px 195px;
  justify-content: center;
  margin: 0 auto;
  font-family: satoshi;

  &__content{
    width: 40%;
    color: white;
  }

  &--svg{
    width: 40%;
    padding-block-end: 10px;
    display: flex;
    justify-content: center;
  }

  &--logo{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    

  }

  &--h1{
    display: flex;
    justify-content: center;
    font-size: 4em;
    font-weight: bold;
  }

  &--h2{
    display: flex;
    justify-content: center;
    font-size: 1.9em;
  }

  &--text{
    display: flex;
    text-align: center;
    font-size: 1.3em;
    padding: 10px 50px;
  }

}

</style>
