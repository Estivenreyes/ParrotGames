<script setup>
  import Mainforum from './components/Mainforum.vue'
  import shop from './components/pages/shop.vue'
</script>

<template>
  <div class="page">
    <header>
      <div class="nav">
        <img alt="Parrot logo" class="logo" src="./assets/img/logo.svg" />
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

    <section class="item">
      <div class="item__container">
        <figure class="item--shop">
          <a href="./components/pages/shop.vue">
            <img src="./assets/img/shopItem.png" alt="shopItem"></a>
          <p class="item--text">Buy video games and support your favorite development.</p>
        </figure>
        <figure class="item--shop">
          <img src="./assets/img/communityItem.png" alt="communityItem">
          <p class="item--text">Socializate with another people that share your passions.</p>
        </figure>
        <figure class="item--shop">
          <img src="./assets/img/createGameItem.png" alt="createGameItem">
          <p class="item--text">Create a developer profile and publish your games to the public.</p>
        </figure>
      </div>
    </section>

    <!--slider here-->
    <!-- <section class="games">
      <h2 class="game--text">Explore a long list of your favorite games</h2>
    </section> -->
    <main>
      <Mainforum/>
    </main>
  </div>

  <footer></footer>
</template>

<style lang="scss">
$blue: #1569DB;
$gray: #2E2E2E;
$nav: #232323;

* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

.page {
  width: 100%;
  font-family: satoshi;
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

.landing {
  background-image: url("../src/assets/img/landingPage.png");
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;

  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 390px 195px;
  justify-content: center;
  margin: 0 auto;
  font-family: satoshi;

  &__content {
    width: 40%;
    color: white;
  }

  &--svg {
    width: 40%;
    padding-block-end: 10px;
    display: flex;
    justify-content: center;
  }

  &--logo {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;


  }

  &--h1 {
    display: flex;
    justify-content: center;
    font-size: 4em;
    font-weight: bold;
  }

  &--h2 {
    display: flex;
    justify-content: center;
    font-size: 1.9em;
  }

  &--text {
    display: flex;
    text-align: center;
    font-size: 1.3em;
    padding: 10px 27px;
  }
}

.item {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
  justify-content: space-around;
  padding: 100px;

  &__container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: center;
    width: 100%;
    margin: 100px;

  }

  &--shop {
    width: 25%;
    text-align: center;
    margin: 50px;
  }

  &--text {
    padding: 20px;
    font-size: 1.3em;
  }
}

// Samsung galaxy S8
@media only screen and (min-width:768px) {}
</style>
